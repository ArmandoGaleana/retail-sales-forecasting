Retail Sales Forecasting

Descripción del proyecto

Proyecto de Data Science enfocado en el análisis histórico y la predicción de ventas en el sector retail.

El objetivo principal fue desarrollar un modelo de Machine Learning capaz de estimar la demanda de productos a partir de datos históricos de ventas, identificando patrones temporales y variables relevantes para mejorar las predicciones.

Objetivos

Analizar el comportamiento histórico de las ventas.

Identificar tendencias y patrones temporales de demanda.

Limpiar y preparar los datos para el modelado.

Construir variables predictoras mediante ingeniería de características.

Entrenar y evaluar un modelo de regresión para predecir ventas futuras.

Dataset

Se utilizó el conjunto de datos Retail Sales Forecasting Data, obtenido de Kaggle.

El dataset contiene información relacionada con:

Ventas históricas.

Productos y catálogo.

Tiendas.

Precios.

Descuentos y promociones.

Información de ventas online.

Tecnologías utilizadas

Python

Pandas

NumPy

Matplotlib

Scikit-learn

Jupyter Notebook

Git y GitHub

Metodología

1. Exploratory Data Analysis (EDA)

Análisis de estructura y dimensiones de los conjuntos de datos.

Identificación de valores nulos y registros duplicados.

Análisis de distribución de ventas.

Identificación de patrones temporales y comportamiento de la demanda.

2. Data Cleaning

Eliminación de registros con cantidades de venta no positivas.

Eliminación de registros con precios negativos.

Conversión de variables temporales al formato datetime.

Selección de variables relevantes para el modelado.

3. Feature Engineering

Se construyeron variables predictoras para representar el comportamiento histórico de las ventas:

Variables temporales: día, mes, año y semana.

Indicador de fin de semana.

Variables históricas: lag_1, lag_7, lag_14 y lag_28.

Promedios móviles: rolling_mean_7 y rolling_mean_28.

4. Model Training

Se entrenó un modelo Random Forest Regressor utilizando una muestra de 500,000 observaciones del conjunto de entrenamiento.

Se realizó una división temporal de los datos:

Entrenamiento: registros anteriores al 1 de julio de 2024.

Prueba: registros desde el 1 de julio de 2024.

5. Model Evaluation

El modelo fue evaluado mediante tres métricas:

Métrica

Resultado

MAE

2.1682

RMSE

5.7622

R²

0.9575

Principales hallazgos

Se identificaron patrones semanales en el comportamiento de las ventas.

Los viernes registraron el mayor promedio de ventas entre los días de la semana.

El historial reciente de ventas fue el principal predictor del modelo.

Las variables lag_1, lag_14 y rolling_mean_7 concentraron la mayor importancia predictiva.

El modelo obtuvo un R² de 0.9575 en el conjunto de prueba.

Conclusiones

El proyecto permitió desarrollar un flujo de trabajo de Machine Learning para la predicción de demanda en retail, desde la exploración y preparación de datos hasta el entrenamiento y evaluación del modelo.

Los resultados muestran que las variables históricas de ventas aportan información relevante para estimar la demanda, ofreciendo una base para futuras mejoras en la planificación de inventario y la toma de decisiones comerciales.

Próximas mejoras

Incorporar explícitamente los días sin ventas.

Comparar el desempeño con otros algoritmos de Machine Learning.

Evaluar estrategias adicionales de ingeniería de características.

Mejorar la evaluación para pronósticos de múltiples días.