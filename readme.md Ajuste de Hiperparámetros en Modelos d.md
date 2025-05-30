# Ajuste de Hiperparámetros en Modelos de Clasificación

Este notebook de Jupyter se enfoca en el ajuste de hiperparámetros para mejorar el rendimiento de los modelos de clasificación en el dataset "diabetes.csv".

## Dataset

El dataset "diabetes.csv" contiene información médica de pacientes y la variable objetivo indica si tienen diabetes o no. Las columnas incluyen:

* `Pregnancies`: Número de embarazos.
* `Glucose`: Concentración de glucosa en plasma.
* `BloodPressure`: Presión arterial diastólica.
* `SkinThickness`: Grosor del pliegue cutáneo del tríceps.
* `Insulin`: Niveles de insulina en suero.
* `BMI`: Índice de masa corporal.
* `DiabetesPedigreeFunction`: Función de pedigrí de diabetes.
* `Age`: Edad.
* `Outcome`: Variable objetivo (1 si tiene diabetes, 0 si no).

## Librerías Utilizadas

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn` (para modelos, división de datos y métricas)
* `optuna` (para optimización de hiperparámetros)

## Metodología

1.  **Carga y Exploración de Datos (EDA):**
    * Se cargó el dataset y se realizó un análisis exploratorio para entender las variables y sus distribuciones.
    * Se analizaron las estadísticas descriptivas y la distribución de la variable objetivo.
2.  **Preprocesamiento de Datos:**
    * Se dividió el dataset en conjuntos de entrenamiento y prueba.
3.  **Modelado y Ajuste de Hiperparámetros:**
    * Se implementaron varios modelos de clasificación:
        * Regresión Logística
        * K-Nearest Neighbors (KNN)
        * Support Vector Machine (SVM)
        * Random Forest
        * Gradient Boosting Machine (GBM)
    * Se utilizó la librería `optuna` para optimizar los hiperparámetros de cada modelo. `Optuna` permite explorar eficientemente el espacio de hiperparámetros y encontrar las mejores combinaciones.
    * Se definió una función objetivo para cada modelo que calcula el rendimiento del modelo (ROC-AUC) en el conjunto de validación.
4.  **Evaluación de Modelos:**
    * Se evaluó el rendimiento de los modelos con los hiperparámetros optimizados en el conjunto de prueba.
    * Se compararon los resultados de los modelos utilizando la métrica ROC-AUC.
    * Se visualizaron los resultados mediante un gráfico de barras.

## Resultados

Se presentan los resultados de la evaluación de los modelos en el conjunto de prueba, comparando el rendimiento (ROC-AUC) de cada modelo después del ajuste de hiperparámetros.

## Conclusiones

Se analizan los resultados del ajuste de hiperparámetros y se discute la importancia de este proceso para mejorar el rendimiento de los modelos de clasificación. Se pueden incluir observaciones sobre qué hiperparámetros fueron más influyentes para cada modelo.