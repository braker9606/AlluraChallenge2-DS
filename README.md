# AlluraChallenge2-DS
Telecom X – Análisis de Evasión de Clientes
Autor: Armando René Cartagena Muñoz
Programa: Especialización en Data Science
Proyecto académico: Challenge Telecom X – Alura

1. Introducción

La evasión de clientes (customer churn) constituye uno de los principales desafíos estratégicos en empresas del sector de telecomunicaciones, debido a su impacto directo en la estabilidad financiera y la sostenibilidad del negocio. La pérdida recurrente de clientes no solo afecta los ingresos, sino que incrementa los costos asociados a adquisición y marketing.

El presente trabajo desarrolla un Análisis Exploratorio de Datos (EDA) orientado a identificar patrones, relaciones y variables potencialmente asociadas al fenómeno de cancelación del servicio en la empresa Telecom X.

Este estudio tiene un enfoque analítico–descriptivo y se enmarca dentro de un ejercicio académico aplicado, con el propósito de sentar las bases para futuros modelos predictivos de clasificación orientados a la anticipación del churn.

2. Planteamiento del problema

La organización enfrenta una tasa significativa de cancelación del servicio. En este contexto, surge la necesidad de responder a la siguiente pregunta de investigación:

¿Qué variables demográficas, contractuales y financieras presentan mayor asociación con la evasión de clientes?

El análisis busca generar evidencia cuantitativa que permita comprender el comportamiento de los usuarios y orientar estrategias de retención basadas en datos.

3. Objetivos
3.1 Objetivo general

Analizar el comportamiento del churn en Telecom X mediante técnicas de análisis exploratorio de datos, con el fin de identificar variables relevantes para la toma de decisiones estratégicas.

3.2 Objetivos específicos

Evaluar la distribución de la variable objetivo (churn).

Analizar la relación entre variables categóricas y la cancelación del servicio.

Comparar variables numéricas entre clientes activos y clientes que cancelaron.

Examinar la correlación entre variables cuantitativas.

Derivar insights estratégicos con potencial aplicación en modelos predictivos.

4. Preparación y tratamiento de datos

El proceso de data wrangling incluyó las siguientes etapas metodológicas:

Extracción de datos desde una API en formato JSON.

Transformación y estructuración en un DataFrame para su manipulación.

Identificación y tratamiento de valores faltantes e inconsistencias.

Conversión de variables numéricas al tipo de dato correspondiente.

Estandarización de variables binarias (Yes/No → codificación homogénea).

Creación de variables derivadas, como Cuentas_Diarias, con el objetivo de enriquecer el análisis financiero.

Estas etapas garantizaron consistencia estructural y calidad mínima de los datos antes del análisis exploratorio.

5. Análisis Exploratorio de Datos (EDA)
5.1 Distribución de la variable objetivo

Se examinó la proporción de clientes que cancelaron el servicio frente a aquellos que permanecen activos, con el fin de evaluar el balance de clases y la magnitud del fenómeno.

El análisis permitió dimensionar la relevancia del churn dentro del conjunto de datos.
5.2 Análisis de variables categóricas

Se estudió la relación entre churn y variables como:

Tipo de contrato

Género

Método de pago

Los resultados evidencian una mayor tasa de evasión en clientes con contratos mensuales, lo cual sugiere que la flexibilidad contractual podría estar asociada a una menor fidelización.

5.3 Análisis de variables numéricas

Para las variables cuantitativas (antigüedad, cargos mensuales, total facturado y cargos diarios) se emplearon diagramas de caja (boxplots), permitiendo comparar:

Mediana

Rango intercuartílico

Dispersión

Valores atípicos

Principales hallazgos:

Los clientes que cancelan presentan menor antigüedad promedio.

El churn se asocia a mayores cargos mensuales.

El total facturado muestra alta dependencia de la antigüedad del cliente.

Estos resultados sugieren que la permanencia en el servicio podría actuar como variable moderadora del riesgo de cancelación.

6. Análisis de correlación

Se construyó una matriz de correlación para evaluar relaciones lineales entre variables numéricas.

Hallazgos relevantes:

La antigüedad presenta correlación negativa con el churn.

Los cargos mensuales y diarios muestran asociación positiva con la evasión.

Existe fuerte correlación entre total facturado y antigüedad, lo cual es consistente con la lógica acumulativa del servicio.

Este análisis permite anticipar posibles problemas de multicolinealidad en futuros modelos predictivos.

7. Conclusiones

El análisis exploratorio evidencia que:

El churn se concentra en clientes de baja antigüedad.

Los contratos mensuales presentan mayor vulnerabilidad a la cancelación.

La permanencia prolongada actúa como factor protector.

El nivel de facturación influye en el comportamiento de abandono.

Estos hallazgos aportan insumos estratégicos para la formulación de políticas de retención y segmentación.

8. Recomendaciones estratégicas

Diseñar incentivos para migrar clientes hacia contratos de mayor duración.

Implementar modelos de alerta temprana durante los primeros meses del cliente.

Evaluar esquemas de beneficios o ajustes tarifarios para clientes con alta facturación.

Avanzar hacia el desarrollo de modelos predictivos supervisados (Logistic Regression, Random Forest, Gradient Boosting) para estimar probabilidad de churn.

9. Tecnologías utilizadas

Python

Pandas

NumPy

Matplotlib

Seaborn

Google Colab

10. Consideraciones finales

Este proyecto fue desarrollado como ejercicio académico aplicado dentro del Challenge Telecom X de Alura, en el marco de la formación en Data Science.

El análisis constituye una fase exploratoria que puede servir como base para la construcción de modelos predictivos y evaluaciones más avanzadas en etapas posteriores del proyecto.
