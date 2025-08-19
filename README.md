# TelecomX_LATAM
# 📊 Telecom X - Análisis de Evasión de Clientes (Churn)

Este proyecto forma parte del desafío de análisis de datos en **Telecom X**, cuyo objetivo es entender los factores que llevan a los clientes a cancelar el servicio (**Churn**).  
El análisis permitirá generar **insights estratégicos** para la empresa y sentar la base para futuros **modelos predictivos**.

---
│## ESTRUCTURA
├── TelecomX_LATAM.ipynb # Cuaderno principal con todo el flujo ETL + EDA + informe
├── TelecomX_Data.json # Dataset con los datos de clientes (fuente original)
└── README.md # Documentación del proyecto

## 🚀 Objetivos del proyecto
- Importar y manipular datos desde una fuente JSON (simulación de API).
- Aplicar **ETL (Extracción, Transformación y Carga)** para preparar los datos.
- Realizar un **Análisis Exploratorio de Datos (EDA)** con visualizaciones.
- Identificar variables clave asociadas a la evasión de clientes.
- Elaborar un **informe final** con hallazgos e insights.

---

## 📂 Estructura del Notebook
1. **Extracción**
   - Subida de archivo `TelecomX_Data.json`.
   - Carga de datos con `pandas`.

2. **Transformación**
   - Normalización de columnas anidadas (`customer`, `phone`, `internet`, `account`).
   - Limpieza de datos y conversión de tipos.
   - Creación de variables planas como `Charges_Monthly` y `Charges_Total`.

3. **Carga y Análisis (EDA)**
   - Distribución de clientes con y sin churn.
   - Relación entre tipo de contrato y churn.
   - Relación entre cargos mensuales y churn.
   - Mapa de correlación entre variables numéricas.

4. **Informe final**
   - Tasa general de churn.
   - Insights principales:
     - Los clientes con contrato **mes a mes** tienen mayor churn.
     - Cargos mensuales altos aumentan la probabilidad de cancelación.
     - Servicios adicionales (seguridad online, soporte técnico) reducen el churn.
     - Contratos de 1 y 2 años muestran mayor retención.
     - Métodos de pago automáticos se asocian a menor churn.

---

## 📊 Ejemplos de gráficos e insights obtenidos

### Gráficos generados:
1. **Distribución de churn vs no-churn** (gráfico de barras).  
2. **Churn según tipo de contrato** (contrato mes a mes muestra mayor churn).  
3. **Boxplot de cargos mensuales vs churn** (clientes con cargos más altos cancelan más).  
4. **Mapa de correlación de variables numéricas**.

### Insights principales:
- Los clientes con contrato **mes a mes** son los que más cancelan.  
- A mayor **cargos mensuales**, mayor probabilidad de churn.  
- Servicios adicionales como **seguridad online y soporte técnico** reducen la tasa de churn.  
- Contratos a **1 y 2 años** muestran mayor retención que contratos mensuales.  
- Métodos de pago **automáticos** (débito automático, transferencia) están asociados con menor churn.

---

## ⚙️ Instrucciones de ejecución

### Requisitos
- Python 3.10+ (o Google Colab).
- Librerías necesarias:
  ```bash
  pip install pandas matplotlib seaborn

---

## 🛠️ Tecnologías utilizadas
- **Python 3.12**
- **Google Colab**
- Librerías:
  - `pandas`
  - `matplotlib`
  - `seaborn`

---

## 📊 Resultados esperados
- 4 gráficos principales que explican el comportamiento de los clientes.
- Un **informe de insights** que permite tomar decisiones estratégicas para disminuir el churn.
- Dataset transformado (`df_flat`) listo para usarse en un modelo de **Machine Learning predictivo**.

---

## 📁 Archivos del proyecto
- `TelecomX_Data.json` → Datos de clientes (fuente principal).
- `TelecomX_diccionario.md` → Diccionario de variables.
- `TelecomX_LATAM.ipynb` → Notebook de análisis.
- `README.md` → Documentación del proyecto.

---

## 👤 Autor
Proyecto realizado por **Alan Ordoñez** como práctica de análisis de datos y EDA en Python.
