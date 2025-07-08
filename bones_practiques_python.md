# Bones pràctiques de Python

Aquest document recull les bones pràctiques recomanades per al desenvolupament de Jupyter Notebooks amb Python de l’especialitat de Data Analytics d’IT Academy.

## Estructura general del notebook

- Assegura’t que el notebook:

  - Tingui un títol clar a la primera cel·la.
  - Inclogui una introducció breu que expliqui l’objectiu de l’arxiu si no hi ha cap README associat.
  - Estigui completament executat, sense errors visibles ni cel·les buides intermèdies.

- Utilitza cel·les **Markdown** per a:

  - Explicar objectius.
  - Justificar decisions.
  - Comentar resultats.
  - Comentar o explicar codi.

No posis explicacions o comentaris dins de cel·les de codi si no són tècnics i específics d’aquell codi.

Per explicar codi, pots fer-ho en cel·les Markdown, per exemple:

    ```python
    # imprimeixo Hola Món
    print('Hola Món')
    ```

Això es veu executat així:
```python
# imprimeixo Hola Món
print('Hola Món')
```

### Convencions generals [PEP](https://elpythonista.com/pep-8)

- Els noms de variables i funcions han de:

  - Estar en minúscules i fer servir guions baixos: ``snake_case``.
  - Ser curts però descriptius: ``edat_usuari``.

- Evita fer servir variables com ``a``, ``x1``, ``data1`` sense context.

- Tots els **imports** han d'anar a la primera cel·la del notebook.

  - Mai importis llibreries dins de funcions.
  - Si alguna llibreria no s'utilitza, elimina-la.

- No deixis mai contrasenyes o claus visibles al notebook.

  - Fes servir variables d’entorn o [fitxers ``.env``](https://davidcasr.medium.com/archivos-env-en-python-c80ec95cb991)  ignorats en Git.
  - Substitueix els valors originals per exemples com ``<your-password>``.

- Mantingues el mateix idioma durant tot el fitxer. 

- No utilitzis ``try-except`` per amagar errors: només per gestionar casos previstos.

### Modularitat i funcions

- Divideix el teu codi en funcions petites i reutilitzables.

  - Una funció ha de tenir una sola responsabilitat.
  - No facis funcions dins d’altres funcions.
  - No combinis entrada, processament i sortida en una sola funció.

- Fes servir ``return`` en totes les funcions, excepte en aquelles que només imprimeixen.

### Errors comuns a evitar

- No facis funcions específiques per a cada entrada o diccionari: fes funcions generals.

- No guardis resultats temporals innecessaris si pots encadenar operacions.

- Si repeteixes una acció, fes servir un bucle (``for``, ``while``) o una funció reutilitzable.

- Si tens molts ``if/elif/else``, considera utilitzar, en aquest ordre de prioritat:

- **Diccionaris** per fer mapes de valors.
- **``match-case``** si utilitzes Python 3.10+ i tens condicions amb ``or``.
- **``if/elif/else``** per tractar rangs de valors.

## Reutilització i eficiència

- Si ja has fet una funció en un exercici anterior, **reutilitza-la**.

- Utilitza funcions integrades de Python (`sum`, `len`, `max`, `min`, etc.).

- Si processes text, aprofita ``re`` (regex) o ``collections.Counter``.

## Neteja de dades

Utilitza expressions regulars per:

- Eliminar caràcters no desitjats.
- Validar correus, dates, etc.


## Documentació i estructura final

- Si no hi ha cap README, el notebook ha de ser **autocontingut**:

  - Títol clar.
  - Introducció breu.
  - Seccions diferenciades.
  - Codi ordenat.

- A les funcions, pots incloure la seva descripció amb un docstring, per exemple:


```python
def convertir_temperatura(valor, unitat):
    """
    Converteix una temperatura en Celsius, Fahrenheit o Kelvin a les altres dues unitats.
    valor: float
    unitat: str - 'C', 'F' o 'K'
    """
```

Aquestes recomanacions estan pensades per ajudar-te a escriure codi més clar, mantenible i professional. Davant del dubte: **menys codi, més llegibilitat**.