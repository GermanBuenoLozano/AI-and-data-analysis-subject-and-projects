# Proyecto de Clasificación de Imágenes con Algoritmos Clásicos de Machine Learning

## Descripción

Este proyecto tiene como objetivo la clasificación de imágenes utilizando algoritmos clásicos de aprendizaje automático. Se emplean modelos como k-Nearest Neighbors (kNN), Árboles de Decisión (DTS), Random Forest y Gradient Boosting para comparar su rendimiento y optimizar la precisión en la clasificación.

## Requisitos

Antes de ejecutar el código, instala las siguientes dependencias:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn opencv-python tqdm
```

## Estructura del Proyecto

```
image_classification_project/
│-- data/                # Carpeta para las imágenes de entrenamiento y prueba
│-- notebooks/           # Jupyter Notebooks con experimentos y análisis
│-- src/
│   │-- preprocess.py    # Procesamiento y limpieza de datos
│   │-- train.py         # Entrenamiento y evaluación de modelos
│   │-- utils.py         # Funciones auxiliares
│-- models/              # Modelos entrenados y resultados guardados
│-- reports/             # Informes y visualizaciones generadas
│-- README.md            # Este archivo
│-- requirements.txt     # Lista de dependencias
```

## Pasos para la Ejecución

### 1. Preparación y Preprocesamiento de Datos

- Carga de imágenes y conversión a escala de grises.
- Normalización y segmentación de imágenes.
- Reducción de dimensionalidad con PCA.

### 2. Entrenamiento y Evaluación de Modelos

Se entrenan y comparan los siguientes algoritmos:

- k-Nearest Neighbors (kNN)
- Árboles de Decisión (DTS)
- Random Forest
- Gradient Boosting

### 3. Ajuste de Hiperparámetros

- Uso de GridSearchCV y RandomizedSearchCV para optimizar el rendimiento de los modelos.

### 4. Evaluación de Modelos

- Cálculo de métricas como accuracy, precision, recall y F1-score.
- Comparación de resultados mediante visualizaciones gráficas.

### 5. Almacenamiento de Modelos y Reportes

- Guardado de modelos entrenados en la carpeta `models/`.
- Generación de informes y visualizaciones en `reports/`.

## Ejemplo de Uso

Para entrenar y evaluar los modelos, ejecuta:

```bash
python src/train.py --dataset data/imagenes --output models/
```

Para visualizar los resultados generados:

```bash
python notebooks/analysis.ipynb
```

## Criterios de Evaluación

- **50%** Ejecución correcta del código y obtención de resultados.
- **30%** Análisis de resultados, propuesta de mejoras y optimización de modelos.
- **20%** Documentación detallada y referencias a herramientas utilizadas, como ChatGPT.

## Contribución

Si deseas contribuir, sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama con tus mejoras (`git checkout -b feature-nueva-funcionalidad`).
3. Realiza tus cambios y súbelos (`git commit -m "Añadida nueva funcionalidad"`).
4. Envía un pull request para revisión.

## Licencia

Este proyecto está bajo la licencia MIT. Puedes usarlo libremente con fines educativos y comerciales.
