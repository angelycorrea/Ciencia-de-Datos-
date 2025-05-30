# Análisis Supervisado de Churn de Clientes de Telecomunicaciones

Este notebook de Jupyter realiza un análisis de clasificación supervisada para predecir el churn (abandono) de clientes en una empresa de telecomunicaciones.

## Dataset

El dataset utilizado es "WA_Fn-UseC_-Telco-Customer-Churn.csv" y contiene información sobre los clientes, los servicios a los que se han suscrito y datos demográficos. Las columnas clave incluyen:

* `Churn`: Variable objetivo que indica si un cliente se fue en el último mes (Sí/No).
* Datos de servicios: Teléfono, múltiples líneas, internet, seguridad en línea, etc.
* Información de la cuenta: Antigüedad, contrato, método de pago, cargos mensuales y totales.
* Información demográfica: Género, si es adulto mayor, tiene pareja y dependientes.

## Librerías Utilizadas

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn` (para modelos, preprocesamiento y evaluación)
* `imblearn` (para manejo de desbalance de clases)

## Metodología

1.  **Carga y Exploración de Datos (EDA):**
    * Se cargó el dataset y se realizó un análisis exploratorio para entender la estructura, tipos de datos y distribuciones de las variables.
    * Se visualizaron las distribuciones de las variables y la relación con la variable objetivo `Churn`.
2.  **Preprocesamiento de Datos:**
    * Se realizó la limpieza de datos, incluyendo el manejo de valores faltantes y la conversión de tipos de datos.
    * Las variables categóricas se codificaron utilizando One-Hot Encoding.
    * Las variables numéricas se estandarizaron.
    * Se dividió el dataset en conjuntos de entrenamiento y prueba.
    * Se aplicó SMOTE (Synthetic Minority Oversampling Technique) para balancear la clase minoritaria (clientes que hicieron churn).
3.  **Modelado:**
    * Se entrenaron y evaluaron varios modelos de clasificación:
        * K-Nearest Neighbors (KNN)
        * Árbol de Decisión
        * Regresión Logística
        * Random Forest
    * Se realizó la optimización de hiperparámetros utilizando GridSearchCV.
4.  **Evaluación de Modelos:**
    * Se evaluó el rendimiento de los modelos utilizando diversas métricas:
        * Matriz de Confusión
        * Reporte de Clasificación (Precisión, Recall, F1-Score)
        * Curva ROC y AUC
    * Se compararon los resultados de los modelos para identificar el mejor desempeño.

## Resultados

Se presenta una comparación del rendimiento de los modelos en términos de precisión, recall y AUC. Se incluye una visualización de las matrices de confusión para cada modelo.

## Conclusiones

Se analizan los resultados obtenidos y se discuten las implicaciones para la predicción del churn de clientes. Se pueden incluir recomendaciones para la empresa basadas en los hallazgos del análisis.
