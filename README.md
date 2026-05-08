# Pipeline de Datos - Ingesta Automatizada
## Descripcion
Script Python que realiza la etapa de ingesta de un pipeline de datos.
Copia archivos CSV desde la carpeta de origen hacia data/raw/ y
registra el proceso con logging.
## Requisitos
- Python 3.8+
- No requiere librerias externas (solo modulos estandar)
## Como ejecutar
python scripts/ingesta.py
## Estructura del proyecto
pipeline_ingesta/
├── data/raw/ -> datos originales copiados
├── scripts/ -> scripts del pipeline
├── logs/ -> registros de ejecucion
└── README.md