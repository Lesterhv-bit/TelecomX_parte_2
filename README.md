Proyecto de Predicción de Churn – Compañía Telefónica

Descripción

Este proyecto tiene como objetivo predecir la cancelación de clientes (churn) en una compañía telefónica y analizar los factores que más influyen en esta decisión. La base de datos utilizada se obtuvo de un trabajo previo de limpieza de datos y contiene información demográfica, de servicios contratados y facturación de 7043 clientes.

Contenido del repositorio

Notebook: churn_analysis.ipynb con todo el código del análisis y los modelos.

Carpeta graficos/: contiene los gráficos generados durante el análisis, guardados en formato PNG para poder visualizarse correctamente en GitHub.

Modelos utilizados

Random Forest: modelo sin normalización, con ajuste de profundidad (max_depth=10).

Detecta bien clientes activos y proporciona estabilidad general.

Regresión Logística: modelo con normalización de variables numéricas.

Prioriza la identificación de clientes que cancelan (mejor recall para churn).

Análisis de variables

Random Forest: identificó como más relevantes account.Charges.Total, customer.tenure, tipo de contrato y servicios adicionales.

Regresión Logística: los coeficientes muestran que contratos cortos, gastos totales bajos y ausencia de servicios aumentan la probabilidad de churn.

Principales hallazgos

Clientes con contratos month-to-month y menor gasto total tienen mayor riesgo de cancelación.

La ausencia de servicios adicionales (Streaming TV, Online Security) incrementa la probabilidad de churn.

Estrategias recomendadas: incentivar contratos de mayor duración, promocionar servicios adicionales y diseñar campañas de retención dirigidas a clientes en riesgo.

Visualizaciones

Gráficos de distribución de churn, matriz de correlación, boxplots y gráficos de importancia de variables.

Todos los gráficos se encuentran en la carpeta graficos/ y se insertan en el notebook con Markdown.
