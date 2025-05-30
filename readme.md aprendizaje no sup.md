# Aprendizaje No Supervisado: Clustering de Pingüinos

Este notebook de Jupyter realiza un análisis de clustering utilizando el algoritmo K-Means para segmentar datos de pingüinos.

## Dataset

El dataset utilizado es "penguins_lter.csv" y contiene información sobre diferentes especies de pingüinos. Las columnas relevantes para el análisis incluyen medidas morfológicas y otras características:

* `Culmen Length (mm)`: Longitud del culmen.
* `Culmen Depth (mm)`: Profundidad del culmen.
* `Flipper Length (mm)`: Longitud de la aleta.
* `Body Mass (g)`: Masa corporal.
* `Delta 15 N (o/oo)`: Delta 15 N.
* `Delta 13 C (o/oo)`: Delta 13 C.

## Librerías Utilizadas

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn` (para preprocesamiento, PCA, K-Means y métricas)

## Metodología

1.  **Carga y Exploración de Datos:**
    * Se cargó el dataset y se realizó una exploración inicial para entender su estructura y tipos de datos.
    * Se manejaron los valores faltantes eliminando las filas que los contenían.
    * Se eliminaron las columnas no numéricas que no eran relevantes para el clustering.
2.  **Preprocesamiento de Datos:**
    * Se escalaron las variables numéricas utilizando `StandardScaler` para asegurar que todas contribuyan por igual al análisis de clustering.
3.  **Reducción de Dimensionalidad (PCA):**
    * Se aplicó Análisis de Componentes Principales (PCA) para reducir la dimensionalidad de los datos a 2 componentes principales, facilitando la visualización y mejorando la eficiencia del clustering.
4.  **Selección de Características:**
    * Se implementaron dos métodos de selección de características:
        * Selección basada en Correlación: Se eliminaron las características altamente correlacionadas para reducir la redundancia.
        * Selección basada en Importancia (SelectKBest): Se seleccionaron las k mejores características utilizando la prueba F.
5.  **Clustering con K-Means:**
    * Se aplicó el algoritmo K-Means para agrupar los datos en clusters.
    * Se utilizó el método del codo para determinar el número óptimo de clusters.
    * Se evaluó la calidad del clustering utilizando el Silhouette Score.
6.  **Comparación de Resultados:**
    * Se compararon los resultados del clustering utilizando los datos originales, los datos transformados por PCA y los datos seleccionados por los diferentes métodos de selección de características.
    * Se visualizaron los clusters en un espacio de 2 dimensiones (usando PCA) para facilitar la interpretación.

## Resultados

Se presentan los resultados del análisis de clustering, incluyendo la visualización de los clusters y la comparación de los Silhouette Scores obtenidos con los diferentes métodos de preprocesamiento y selección de características.

## Conclusiones

Se analizan los resultados del clustering y se discuten las implicaciones para la segmentación de los pingüinos en grupos basados en sus características. Se pueden incluir observaciones sobre la efectividad de los diferentes métodos de preprocesamiento y selección de características en el contexto del clustering.