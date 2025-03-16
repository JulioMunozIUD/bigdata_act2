# bigdata_act2

## Clonar el Repositorio

* https://github.com/JulioMunozIUD/bigdata_act2.git

## Crear y Activar un Entorno Virtual

* python -m venv venv
* source venv/bin/activate  # En Linux/Mac
* venv\Scripts\activate     # En Windows

## Instalar Dependencias

* pip install --upgrade pip
* pip install -e .

## Ejecución del Script de Limpieza

### El script realiza las siguientes acciones:

* Carga datos desde ingestion.db.

* Realiza análisis exploratorio.

* Identifica y elimina duplicados.

* Sustituye valores vacíos y nulos.

* Ajusta tipos de datos según un esquema definido.

* Guarda los datos limpios en cleaned_data.xlsx.

* Genera un informe de auditoría en cleaning_report.txt.

## Workflow Automatizado en GitHub Actions

### El proceso de preprocesamiento y limpieza se ejecuta automáticamente en GitHub Actions    cuando hay un push en la rama main. El workflow bigdata.yml sigue los siguientes pasos:

* Clonar el repositorio.

* Configurar Python en la versión 3.9.2.

* Crear y activar un entorno virtual.

* Actualizar pip e instalar las dependencias.

* Ejecutar cleaning.py.

* Generar y almacenar los archivos resultantes.

* Realizar un commit automático con los cambios generados.
