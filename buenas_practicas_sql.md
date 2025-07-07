# Buenas prácticas de SQL para la especialidad de Data Analytics

Este documento recoge las principales recomendaciones para la redacción, presentación y justificación de consultas SQL en el marco de las entregas de la especialidad de Data Analytics de IT Academy.

## Presentación de las consultas

Para cada consulta entregada:

- Debes asegurarte de mostrar mediante una captura de pantalla tres elementos:

    - La query (consulta): en el bloque de código SQL.
    - El Results Grid: la tabla con los resultados que arroja la consulta.
    - El Action Output: donde se muestra el número de filas afectadas y posibles errores.

    Como el ejemplo que te mostramos a continuación:

    ![alt text](./images/screenshot-query.png)

    Estos tres elementos deben ir en cada respuesta de las prácticas en un solo PDF. 

- Cantidad de soluciones: Si entregas varias soluciones, solo se corregirá la primera que aparezca. Elige la más adecuada y, si lo deseas, puedes justificar por qué descartas otras.

- Justifica solo si consideras que tomaste una decisión poco obvia, por ejemplo: "uso subconsulta porque me permite...", "prefiero esta función por...", "selecciono las transacciones no declinadas por...", etc.

## Recomendaciones técnicas en SQL

### Estilo y legibilidad

- Utiliza mayúsculas para las palabras reservadas de SQL (``SELECT``, ``JOIN``, ``WHERE``, ``GROUP BY``...).
- Utiliza minúsculas para los nombres de tablas y columnas (company_id, transaction_date, etc.).
- Usa sangrías y saltos de línea para que la consulta sea legible.
- Asigna alias a las tablas (c, t, u...) y mantén el uso de esos alias consistente en toda la query.
- Elige alias y nombres de columnas calculadas claros y sin espacios (total_ventas, media_gasto).
- Mantén el mismo idioma durante toda la query.

### Consultas y estructuras

- Evita subconsultas si el enunciado no las exige. Prefiere JOIN por rendimiento y claridad.
- Si el enunciado exige subconsultas, úsalas aunque puedas hacerlo con JOIN.
- Utiliza ``USE <nombre_bbdd>``; al principio del script si trabajarás con una sola base de datos.
- Si usas varias tablas, sé consistente con los llamados. Tienes dos opciones:
    1. Donde las llamas sin necesidad de especificar las tablas ``columna``, con la excepción que haya coincidencia del nombre de columnas ``tabla.id`` por ejemplo.
    2. Donde las llamas siempre con las tablas a las que corresponde ``tabla.columna``. 
    
    Lo que no se debe hacer es combinarlo, que a veces se agregue la tabla y a veces no, esto no se hace!

### Operaciones

- Si estás trabajando con dinero, redondea a dos decimales con ``ROUND(columna, 2)`` o ``FORMAT(columna, 2)``.
- Utiliza funciones como ``STR_TO_DATE``, ``DATE_FORMAT``, ``LEFT``, ``RIGHT``, ``CAST``, ``CONCAT``, según lo que se te pida para manipular o transformar los datos.
- Controla el uso de ``CASCADE``. Solo debe usarse si tiene sentido borrar en cascada (como facturas y sus líneas) y si tienes control absoluto de la DB.

### Archivos .SQL portables

Entrega tu archivo .sql de forma que, si se ejecuta en otro ordenador, reproduzca el mismo entorno:

- Crea la base de datos.
- Usa ``DROP IF EXISTS`` para evitar errores si ya existe.
- Incluye la creación de tablas.
- Incluye los ``INSERT INTO``, cargas desde archivos o al menos un comentario con ``-- `` que en ese punto se debe ejecutar un .sql.

### Recomendaciones adicionales

- Nunca uses ``SET FOREIGN_KEY_CHECKS = 0``. Esto desactiva la integridad referencial y puede ocultar errores graves.
- No utilices ``SAFE_UPDATES = 0`` para saltarte restricciones de seguridad. Asegúrate de incluir ``WHERE`` y/o ``LIMIT`` en ``DELETE`` o ``UPDATE``.
- Evita ``IN`` o ``LIKE`` si puedes usar ``=``, ``EXIST`` o ``JOIN``. ``IN`` puede ser más costoso o ambiguo en ciertos casos.

### Herramientas recomendadas para complementar

- En Workbench: *Database → Reverse Engineer o Models → Create EER Model from Database*: para mostrar el diagrama o modelo de la DB.
- [Draw.io](https://app.diagrams.net/) para representar esquemas EER.
- YouTube: [STR_TO_DATE()](https://www.youtube.com/watch?v=z2_8cYcxfwg) explicado.