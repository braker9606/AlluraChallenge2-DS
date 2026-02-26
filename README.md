# AlluraChallenge2-DS
Telecom X – Análisis de Evasión de Clientes
Autor: Armando René Cartagena Muñoz
Programa: Especialización en Data Science
Proyecto académico: Challenge Telecom X – Alura

## 📌 Descripción del proyecto

La evasión de clientes (customer churn) representa uno de los principales desafíos estratégicos en la industria de telecomunicaciones, debido a su impacto directo en los ingresos y en la sostenibilidad del negocio.

Este proyecto desarrolla un Análisis Exploratorio de Datos (EDA) sobre la base de clientes de Telecom X, con el objetivo de identificar patrones, relaciones y variables asociadas a la cancelación del servicio.

El análisis constituye la fase inicial para la construcción futura de modelos predictivos de clasificación orientados a la estimación de probabilidad de churn.

## 🎯 Objetivos
Objetivo general

Analizar el comportamiento de la evasión de clientes mediante técnicas de análisis exploratorio de datos, con el fin de identificar factores relevantes para la toma de decisiones estratégicas.

### Objetivos específicos

 - Evaluar la distribución de la variable objetivo (churn).

 - Analizar la relación entre variables categóricas y la cancelación del servicio.

 - Comparar variables numéricas entre clientes que evaden y clientes que permanecen.

 - Examinar correlaciones entre variables cuantitativas.

 - Generar insights estratégicos con potencial aplicación en modelos predictivos.

## 📂 Descripción del conjunto de datos

El conjunto de datos fue obtenido mediante una API en formato JSON e incluye información relacionada con:

Datos demográficos

Tipo de contrato

Métodos de pago

Información de facturación

Uso de servicios

Variable objetivo: Churn

## 🧹 Preparación y limpieza de datos

El proceso de preprocesamiento incluyó:

 - Extracción y transformación de datos desde JSON a DataFrame.

 - Identificación y tratamiento de valores faltantes.

 - Corrección de tipos de datos en variables numéricas.

 - Estandarización de variables binarias (Yes/No).

 - Creación de variables derivadas (por ejemplo, Cargos_Diarios).

Estas etapas garantizaron coherencia estructural y calidad analítica antes de realizar el análisis exploratorio.

📊 Análisis Exploratorio de Datos (EDA)
1️⃣ Distribución del churn

Se evaluó la proporción de clientes que cancelaron el servicio frente a aquellos que permanecen activos, permitiendo dimensionar la magnitud del fenómeno.

2️⃣ Análisis de variables categóricas

Se examinó la relación entre churn y:

 - Tipo de contrato

 - Género

 - Método de pago

Hallazgo relevante:
Los contratos mensuales presentan una tasa de evasión significativamente mayor que los contratos de largo plazo.

3️⃣ Análisis de variables numéricas

Variables analizadas:

 - Antigüedad (Tenure)

 - Cargos mensuales

 - Cargos totales

 - Cargos diarios (variable derivada)

Se utilizaron diagramas de caja (boxplots) para comparar:

 - Mediana

 - Dispersión

 - Rango intercuartílico

 - Valores atípicos

### Principales resultados:

Los clientes con menor antigüedad presentan mayor probabilidad de evasión.

Los cargos mensuales elevados se asocian positivamente con el churn.

Existe fuerte relación entre cargos totales y antigüedad.

## 🔗 Análisis de correlación

Se construyó una matriz de correlación para evaluar relaciones lineales entre variables numéricas.

Observaciones principales:

- Relación inversa entre antigüedad y churn.

- Asociación positiva entre cargos mensuales y evasión.

- Alta correlación entre cargos totales y antigüedad.

- Este análisis permite anticipar posibles efectos de multicolinealidad en futuros modelos predictivos.

## 📈 Insights estratégicos

El churn se concentra en clientes recientes con contratos mensuales.

La antigüedad actúa como factor protector.

El nivel de facturación influye en el comportamiento de abandono.

Las variables contractuales y económicas son determinantes clave.

## 🚀 Trabajo futuro

Implementación de modelos supervisados:

Regresión Logística

Random Forest

Gradient Boosting

Evaluación mediante métricas:

ROC-AUC

Matriz de confusión

Precision y Recall

Análisis de importancia de variables.

Construcción de un pipeline de predicción de churn.

## 🛠️ Tecnologías utilizadas

- Python 3.x

- Pandas

- NumPy

- Matplotlib

Google Colab
