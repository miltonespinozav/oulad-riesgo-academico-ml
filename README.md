# Predicción de riesgo académico estudiantil con OULAD

## Descripción del proyecto

Este repositorio contiene el desarrollo de la Tarea 1 del módulo **MTDI202: Big Data, Analytics & Data Scientist**. El proyecto aplica limpieza de datos, manejo de DataFrames, análisis exploratorio de datos, visualización y un modelo básico de Machine Learning supervisado para identificar estudiantes con posible riesgo académico en entornos virtuales de aprendizaje.

## Autor

**Milton Elías Espinoza Villalba**

## Dataset

Se utiliza el **Open University Learning Analytics Dataset (OULAD)**, un dataset público y anonimizado que contiene información sobre estudiantes, cursos, evaluaciones e interacciones con un entorno virtual de aprendizaje.

Fuente principal: UCI Machine Learning Repository / Open University Learning Analytics Dataset.

## Problemática analítica

En contextos de educación virtual, el bajo rendimiento académico y el retiro estudiantil pueden detectarse tarde. Este proyecto busca analizar patrones de comportamiento y desempeño que permitan clasificar a los estudiantes en dos grupos:

- **Riesgo académico:** estudiantes con resultado final `Withdrawn` o `Fail`.
- **Sin riesgo académico:** estudiantes con resultado final `Pass` o `Distinction`.

## Objetivo

Desarrollar un notebook en Google Colab que integre limpieza, transformación, análisis exploratorio, visualización y Machine Learning básico para predecir riesgo académico estudiantil.

## Herramientas utilizadas

- Python
- Google Colab
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Estructura del repositorio

```text
oulad-riesgo-academico-ml/
│
├── README.md
├── notebooks/
│   └── notebook_eda_ml_riesgo_academico_oulad.ipynb
├── data/
│   └── instrucciones_descarga_dataset.md
├── outputs/
│   └── resultados_modelo.csv
└── informe/
    └── informe_final_riesgo_academico.pdf
```

## Metodología

1. Carga de librerías.
2. Descarga y lectura del dataset.
3. Revisión inicial de tablas.
4. Limpieza de datos.
5. Integración de DataFrames.
6. Creación de variable objetivo.
7. Análisis exploratorio de datos.
8. Visualizaciones.
9. Entrenamiento de modelos supervisados.
10. Evaluación con métricas de clasificación.
11. Interpretación de resultados.

## Modelo de Machine Learning

El problema se formula como **clasificación supervisada**. Se comparan modelos básicos como:

- Regresión logística.
- Random Forest Classifier.

Las métricas utilizadas son:

- Accuracy.
- Precision.
- Recall.
- F1-score.
- Matriz de confusión.
- ROC AUC, cuando aplica.

## Cómo ejecutar el notebook

1. Abrir Google Colab.
2. Subir el notebook ubicado en la carpeta `/notebooks`.
3. Ejecutar las celdas en orden.
4. Si la descarga automática del dataset falla, descargar manualmente el ZIP desde UCI Machine Learning Repository y subirlo a Colab.
5. Revisar los resultados, gráficos y métricas.
6. Actualizar el informe final en PDF con los resultados obtenidos.

## Nota ética

El dataset es público y anonimizado. Las predicciones del modelo deben entenderse como apoyo para la toma de decisiones educativas, no como mecanismo automático de sanción o exclusión estudiantil.