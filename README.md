# 📊 Análisis de Churn - Telecom X | Challenge Data Science Alura Latam

Este proyecto forma parte de un desafío de **Alura Latam**, donde se asume el rol de analista de datos para la empresa **Telecom X**. El objetivo principal es identificar los factores que impulsan la evasión de clientes (**Churn Rate**) y preparar un dataset optimizado para que el equipo de Ciencia de Datos desarrolle modelos predictivos.

---

## 📝 Contexto del Proyecto

Telecom X enfrenta un alto índice de rotación de clientes sin una causa clara identificada. El análisis se centra en el comportamiento de los usuarios, sus tipos de contrato, métodos de pago y cargos financieros para extraer insights que permitan diseñar estrategias de retención efectivas.

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Python 3.x
* **Entorno:** Google Colab
* **Librerías:**
    * `Pandas`: Extracción, limpieza y manipulación de datos.
    * `Matplotlib` & `Seaborn`: Visualización de datos y análisis estadístico gráfico.
    * `Requests`: Consumo de datos desde API (JSON).

## 🚀 Fases del Proyecto

### 1. Extracción y Transformación (ETL)
* **Carga:** Importación de datos desde una API en formato JSON y normalización de campos anidados.
* **Limpieza:** Tratamiento de valores nulos, corrección de tipos de datos (específicamente la conversión de `Total_Charges` a float) y eliminación de registros inconsistentes en la variable objetivo.
* **Feature Engineering:** Creación de la métrica `account_Charges_Daily` para analizar el impacto del costo diario por cliente.

### 2. Análisis Exploratorio de Datos (EDA)
Se realizaron diversas visualizaciones para identificar patrones críticos:
* **Distribución de Churn:** Identificación de la tasa base de evasión (26.5%).
* **Análisis por Segmentos:** Evaluación de la fuga según tipo de contrato, género y métodos de pago.
* **Análisis Numérico:** Estudio de la correlación entre la antigüedad (`tenure`) y el abandono del servicio.

## 📈 Hallazgos Clave

* **Zona de Riesgo:** Los clientes nuevos (0-6 meses) tienen la mayor probabilidad de fuga.
* **Tipo de Contrato:** Los contratos mensuales ("Month-to-month") son la principal vía de evasión.
* **Sensibilidad al Precio:** Los clientes con cargos mensuales superiores a $80 presentan una mayor tasa de cancelación.
* **Método de Pago:** El pago mediante cheque electrónico está fuertemente asociado con el Churn.

## 💡 Recomendaciones Estratégicas

1.  Implementar un programa de **Onboarding** para clientes en sus primeros 6 meses.
2.  Incentivar la migración de contratos mensuales a **contratos anuales**.
3.  Fomentar el uso de **pagos automáticos** para reducir la fricción en el proceso de cobro.
4.  Revisar la propuesta de valor para los planes premium de alto costo.

---

## 👤 Autor
**Luis Alejandro Mamani Garnique** *Estudiante de Ingeniería Industrial en la UNMSM (8vo ciclo).* *Estudiante del grupo G9 ORACLE NEXT GENERATION.* *Practicante de Gestión y Control de Información en el área de Operaciones.* *Interesado en la Ciencia de Datos y la Analítica aplicada a la optimización de procesos.*

---

## 🚀 Instrucciones para Ejecutar
1. Clonar el repositorio: `git clone https://github.com/Panchito1602/Alura-Latam-DataScience-Challenge-1`
2. Abrir el archivo `.ipynb` en **Google Colab**.
3. Ejecutar las celdas en orden para cargar los datasets desde el repositorio de Alura y visualizar los gráficos generados.

---
