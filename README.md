# firearm_analysis_project

## Descripción general

Este proyecto tiene como objetivo analizar las verificaciones de los antecedentes de las armas de fuego en los Estados Unidos. Procesa y examina datos sobre permisos de armas de fuego, ya sean armas de corto y largo alcance, por estado y año. El proceso y examen también proporciona información sobre tendencias y patrones en diferentes estados.

## Características

- Leer y limpiar datos de archivos CSV.
- Procesar información de fecha para un mejor análisis.
- Agrupar datos por estado y año para obtener información agregada.
- Identificar los años y los estados con el mayor número de permisos y ventas de armas de fuego.
- Realizar análisis temporales para comprender las tendencias a lo largo del tiempo.
- Realizar análisis de los estados  y manejar valores atípicos.
- Fusionar datos con información de la población para comparaciones relativas.

## Instalación

### Prerrequisitos

- Python 3.6 o superior
- Pip (Paquete instalador de Python)

### Pasos

1. Puede clonar el repositorio o descargar los archivos del proyecto:
	```bash
	git clone https://github.com/meland87/firearm_analysis_project.git
	cd firearm_analysis_project
	```

2. Instalar los requisitos de dependencia:
	```bash
	pip  install -r requirements.txt
	```

3. Instalar el paquete en modo editable:
	```bash
	pip install -e .
	´´´

## Uso 

### Ejecución del análisis

Puedes ejecutar el fichero main directamente:

```bash
python main.py
```

Alternativamente, usa la consola del script definida en `setup.py`:

```bash
firearm_analysis
```

### Ejecución de funciones individuales

El script `main.py`esta implementado para ejecutar todas las funciones secuencialmente. Aunque puedes ejecutar las funciones individualmente llamando directamente a esta en un intérprete de Python u otro script.

### Ejemplo

```python
from main import read_csv, clean_csv, ...

# Lectura de datos
firearm_data = read_csv('data/nics-firearm-background-checks.csv')

# Clean data
firearm_data_cleaned = clean_csv(firearm_data)
# Continuación con otras funciones...
```
# ¡¡¡Importante!!!

A partir de la función del ejercicio 3.3 hay que trabajar con el dataframe devuelto por aquel del ejercicio 1.3. Ello evitará inconsistencias en el nombre de la columna longgun.

## Datos

### Antecedentes de armas de fuego

- **Fichero**: `data/nics-firearm-background-checks.csv`
- **Fuente**: [Kaggle](https://www.kaggle.com/datasets/pedropereira94/nics-firearm-background-checks)
- **Descripción**: Este dataset contiene información sobre los antecedentes para las armas de fuego con permisos, pistolas y armas largas por por fecha y estado.

### Poblaciones estado

- **Fichero**: `data/us-state-populations.csv`
- **Fuente**: [Git](https://gist.githubusercontent.com/bradoyler/0fd473541083cfa9ea6b5da57b08461c/raw/fa5f59ff1ce7ad9ff792e223b9ac05c564b7c0fe/us-state-populations.csv)
- **Descripción**: Este dataset contiene la población de los diferentes estados de EE.UU. del año 2014.

## Salidas

Los scripts generan varios tipos de salidas, incluyendo:

- La consola puede obtener los logs para cada paso.
- Dibuja tendencias a lo largo del tiempo.
- Mensajes informativos identificando estados con las actividades de armas de fuego más altas
- Datos ajustados después de manejar los datos atípicos.
- Reflexiones subjetivas por parte del autor valorando los argumentos dibujados y las operaciones de cálculo.

## Tests

### Ejecución de los tests

Para ejecutar los tests y comprobar la cobertura, sigue los siguientes pasos:

1. Asegúrate de que `pytest` está instalado:
	```bash
	pip install pytest
	```
2. Ejecución de los tests:
	```bash
	pytest
	```
3. Comprobación cobertura del test (si la cobertura está configurada):
	```bash
	pytest --cov=firearm_analysis_project
	```

### Cobertura del test

El test de cobertura provee detalles en las partes del código que son probadas.

## Contribución

¡Las contribuciones son bien recibidas! Hay que bifurcar el repositorio y crear una solicitud de exrtacción con sus cambios.

## Licencia

Este proyecto se ha implementado bajo la licencia del MIT. Ver la [LICENSE](LICENSE)

## Contacto

Para cuestiones o sugerencias, por favor contacte con el mantenedor del proyecto:

- Nombre: Manuel Martín Ela Ndong
- Email: melan@uoc.edu
- Github: [meland87](https://github.com/meland87/firearm_analysis_project)

---

¡Gracias por el interés mostrado en el Proyecto de Análisis de las Armas de Fuego! Espero que le proporcione el conocimiento deseado sobre las verificaciones de los antecedentes de las armas de fuego en los Estados Unidos
