# Buenas prácticas de Python para la especialidad de Data Analytics

Este documento recoge las buenas prácticas recomendadas para el desarrollo de Jupyter Notebooks con Python de la especialidad de Data Analytics de IT Academy.


## Estructura general del notebook

* Asegúrate de que el notebook:

  * Tenga un título claro en la primera celda.
  * Incluya una introducción breve que explique el objetivo del archivo si no hay un README asociado.
  * Esté completamente ejecutado, sin errores visibles ni celdas vacías intermedias.

* Utiliza celdas **Markdown** para:

  * Explicar objetivos.
  * Justificar decisiones.
  * Comentar resultados.
  * Comentar o explicar código.

No coloques explicaciones o comentarios dentro de celdas de código si no son técnicos y únicos del código. 

Para explicar código lo puedes hacer en celdas Markdown, por ejemplo:

    ```python
    # imprimo Hola Mundo
    print('Hola Mundo')
    ```

Esto lo vemos ejecutado así:
```python
# imprimo Hola Mundo
print('Hola Mundo')
```


## Convenciones generales [PEP](https://elpythonista.com/pep-8)

* Los **nombres de variables y funciones** deben:

  * Ser en minúsculas y usar guiones bajos: `snake_case`.
  * Ser cortos pero descriptivos: `edad_usuario`.

* Evita usar variables como `a`, `x1`, `data1` sin contexto.

* Todos los **imports** deben ir en la primera celda del notebook.

  * Nunca importes librerías dentro de funciones.
  * Si alguna librería no se utiliza, elimínala.

* Nunca dejes claves o contraseñas visibles en el notebook.

  * Usa variables de entorno o [archivos `.env`](https://davidcasr.medium.com/archivos-env-en-python-c80ec95cb991) ignorados en Git.
  * Sustituye los valores originales por ``<your-password>`` por ejemplo. 


## Modularidad y funciones

* Divide tu código en **funciones pequeñas y reutilizables**.

  * Una función debe tener una sola responsabilidad.

* No hagas funciones dentro de funciones.

* No combines entrada, procesamiento y salida en una sola función.

* Usa `return` en todas las funciones, excepto en funciones cuyo único fin sea imprimir.

## Errores comunes a evitar

* No hagas funciones específicas para cada entrada o cada diccionario: haz funciones generales.
* No guardes resultados temporales innecesarios si puedes encadenar operaciones.
* Si repites una acción, haz un bucle (`for`, `while`) o una función reutilizable.
* Si tienes muchos `if/elif/else`, considera usar con prioridad:

  1. **Diccionarios** para mapear valores.
  2. **`match-case`** si usas Python 3.10+ y tienes condiciones ``or``.
  3. **`if/elif/else`** para rangos.  

## Seguridad y buenas costumbres

* Nunca subas contraseñas, tokens o claves en cédulas de código.
* Nunca uses `try-except` para ocultar errores: solo para manejar casos previstos.

## Reutilización y eficiencia

* Si ya hiciste una función en un ejercicio anterior, **reutilízala**.
* Usa funciones integradas de Python (`sum`, `len`, `max`, `min`, etc.).
* Si procesas texto, aprovecha `re` (regex) o `collections.Counter`.


## Limpieza de datos

* Usa expresiones regulares para:

  * Eliminar caracteres no deseados.
  * Validar correos, fechas, etc.


## Documentación y estructura final

* Si no hay README, el notebook debe ser **autocontenible**:

  * Título claro.
  * Breve introducción.
  * Secciones diferenciadas.
  * Código ordenado.

* Si entregas funciones que van a ser usadas por otros, incluye docstrings:

```python
def convertir_temperatura(valor, unidad):
    """
    Convierte una temperatura en Celsius, Fahrenheit o Kelvin a las otras dos unidades.
    valor: float
    unidad: str - 'C', 'F' o 'K'
    """
```

Estas recomendaciones están pensadas para ayudarte a escribir código más claro, mantenible y profesional. Ante la duda: **menos código, más legibilidad**.