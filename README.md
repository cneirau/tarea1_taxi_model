# Análisis de Viajes en Taxi en NYC el año 2020

En el presente repositorio se realizó la tarea 1 de la asignatura Desarrollo de Poryectos y Productos de Datos, cuyo propósito fue construir un repositorio en Github para reproducir el código del notebook llamado 00_nyc_taxi_model pero siguiendo las buenas prácticas vistas en el curso y desarrollar una estrategia para explicar y/o demostrar el comportamiento distinto del modelo para cada mes de análisis. El análisis incluyó la comparación de las distribuciones de conjuntos de datos mes a mes durante el primer semestre del año 2020 utilizando la prueba de Kolgomorov-Smirnov y luego se evaluó el desempeño del modelo a lo largo de los 12 meses utilizando como métrica el f1-score.

## Estructura del Repositorio

- `src/` : Carpeta que contiene scripts Python para el procesamiento de datos y la extracción de características.
  - `data/dataset.py` : Script para cargar y preparar los datos.
  - `features/features.py` : Script para construir características y comparar distribuciones.

- `notebooks/` : Carpeta que contiene notebooks Jupyter para la evaluación y análisis del modelo.
  - `00_nyc_taxi_model.ipynb` : Notebook principal para la evaluación del modelo.

- `models/` : Carpeta que contiene el modelo entrenado.
  - `random_forest.joblib` : Modelo de clasificación random forest guardado.

- `.gitignore` : Archivo para excluir archivos y carpetas del control de versiones.
- `README.md` : Este archivo.
- `requirements.txt` : Archivo con los paquetes necesarios para ejecutar el análisis.

## Requisitos

Asegúrate de tener instalado Python 3.9 y pip. Los paquetes necesarios están listados en el archivo `requirements.txt`.

## Configuración

1. Clona el Repositorio
```bash
git clone https://github.com/tu_usuario/tarea1_taxi_model.git
cd tarea1_taxi_model

2. Instala los Requisitos
```bash
pip install -r requirements.txt

## Ejecución

- Abre el notebook 00_nyc_taxi_model.ipynb en Jupyter Notebook o Google Colab.
- Asegúrate de que los datos estén cargados y el modelo esté disponible en la carpeta models/.
- Ejecuta las celdas para cargar los datos mensuales y preprocesarlos. Los datos se cargan usando la función load_data del archivo dataset.py que se encuentra disponible en src/data.
- Ejecuta las celdas para realizar la comparación de distribuciones mes a mes durante todo el primer semestre.
- Ejecuta las celdas para aplicar el modelo random forest a los datos de cada mes y luego graficar el comportamiento mensual durante el año 2020.
