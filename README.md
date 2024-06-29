
# Statical_Learning_Project: Clasificación del Puntaje de Crédito

Este proyecto tiene como objetivo crear un modelo de clasificación del puntaje de crédito de un cliente utilizando técnicas de aprendizaje supervisado. Consiste en tres notebooks: uno para limpieza y análisis exploratorio de datos (EDA), otro para la creación de un pipeline de ingeniería de características y el último para el modelamiento, entrenamiento y evaluación.

## Notebooks

### 1. Limpieza y Análisis Exploratorio de Datos (Cleaning & EDA) - (Proyecto_Statical_1)
- El notebook `Proyecto_Statical_1.ipynb` contiene el proceso de limpieza de datos y análisis exploratorio para comprender la estructura y distribución de los datos financieros.
- Se realizan tareas como la identificación y ajuste del formato de los datos, la detección y tratamiento de datos basura, y la visualización de las características relevantes mediante análisis univariado, bivariado y multivariado.

### 2. Pipeline de Ingeniería de Características (Feature Engineering Pipeline) - (Proyecto_Statical_2)
- El notebook `Proyecto_Statical_2.ipynb` se centra en la creación de un pipeline de ingeniería de características para preparar los datos para el modelado.
- Se implementan técnicas como la imputación de datos faltantes, codificación de variables categóricas, tratamiento de valores atípicos, la normalización o estandarización de características numéricas, su escalado y la creación de nuevas características.

### 3. Modelling - (proyecto_fase_2)
#### 3.1 Preprocesamiento de Datos
- Selección de Características: Se utilizó la información mutua (MI) para seleccionar las características más relevantes para el problema de clasificación.
- Escalado de Características: Se aplicó StandardScaler a las características numéricas para asegurar que todas tuvieran una escala similar.
- Codificación de Variables Categóricas: Se utilizó OneHotEncoder para codificar las variables categóricas. (Opcional si ya estan codificadas)

### 3.2 Modelos de Clasificación Evaluados
Se entrenaron y evaluaron los siguientes modelos de clasificación:

- Gaussian Naive Bayes (GNB)
- Linear Discriminant Analysis (LDA)
- Regresión Logística
- Árbol de Decisión
- Random Forest
- Quadratic Discriminant Analysis (QDA)
- AdaBoost
- Gradient Boosting
- XGBoost
- LightGBM
- Optimización de Hiperparámetros
- Para cada modelo, se exploraron diferentes combinaciones de hiperparámetros utilizando bucles for para encontrar la configuración óptima. Se utilizó la precisión como métrica principal de evaluación.

#### 3.3 Modelos de Ensemble
Se crearon dos modelos de ensemble para combinar las predicciones de los mejores modelos individuales:

- Stacking: Se utilizó una regresión logística como meta-clasificador para combinar las predicciones de los modelos base.
- Soft Voting: Se promediaron las probabilidades de clase de los modelos base para obtener la predicción final.

### 3.4 Resultados
Los resultados de todos los modelos y sus configuraciones de hiperparámetros se guardan en el archivo resultados_modelos.xlsx. El modelo con el mejor rendimiento en el conjunto de prueba fue [indicar el mejor modelo y su precisión].

### 3.5 Exclusión del Modelo SVM
Debido a las limitaciones de recursos computacionales y al tiempo de entrenamiento excesivo, el modelo SVM fue excluido del análisis. A pesar de aplicar diversas técnicas de optimización, el entrenamiento del SVM seguía siendo significativamente más lento que el de otros modelos, y su rendimiento no era sustancialmente mejor.

## Dataset
- El conjunto de datos utilizado contiene información financiera de clientes, incluyendo variables como ingresos, deudas, historial crediticio, entre otras.
- Este conjunto de datos se utiliza para entrenar y evaluar el modelo de clasificación del puntaje de crédito.

## Uso
1. Descarga los notebooks y el conjunto de datos.
2. Abre los notebooks en tu entorno de Jupyter Notebook o JupyterLab.
3. Ejecuta las celdas de código secuencialmente para reproducir el análisis y la creación del modelo.
4. Experimenta con diferentes técnicas y parámetros para mejorar el rendimiento del modelo.

## Contribución
¡Las contribuciones son bienvenidas! Si deseas mejorar el proyecto, puedes abrir una solicitud de extracción con tus cambios.


