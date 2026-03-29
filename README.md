# Airline Loyalty Program Analysis ✈️

Este proyecto realiza un análisis de datos end-to-end sobre el comportamiento de clientes de una aerolínea, cubriendo desde el preprocesamiento técnico hasta la visualización de insights de negocio.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python 3.10+
* **Librerías de Datos:** `pandas`, `numpy`.
* **Visualización:** `seaborn`, `matplotlib`.
* **ML & Preprocesamiento:** `scikit-learn` (`SimpleImputer`).

## 📋 Fases del Proyecto

### 1. Extracción y Limpieza:
* **Normalización:** Estandarización de columnas.
* **Tratamiento de Anomalías:** Corrección de valores negativos en la variable `salary`.
* **Imputación de Nulos:** Uso de `SimpleImputer(strategy='median')` para la columna `salary` (25% de nulos), elegida por su robustez frente a outliers.git
* **Unión de Fuentes:** Merge de `Customer Flight Activity` y `Customer Loyalty History` mediante `loyalty_number`.

### 2. Análisis Exploratorio (EDA)
* **Estadística Descriptiva:** Análisis de medidas de tendencia central y dispersión.
* **Correlación:** Evaluación mediante el coeficiente de Spearman para detectar redundancias (ej. `distance` vs `points_accumulated`).
* **Detección de Outliers:** Identificación de valores atípicos en datos numéricos `clv` y `salary` mediante el método IQR.

### 3. Visualización
* **Análisis Temporal:** Lineplots para detectar estacionalidad en vuelos.
* **Segmentación:** Boxplots de salario por educación y gráficos de barras agrupados por género/estado civil.
* **Composición:** Pie plot para la distribución de niveles de fidelidad (tarjetas).

## 🚀 Instrucciones de Uso

1. **Instalar Dependencias:**
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn
Estructura de Archivos:
Asegúrate de tener los archivos Customer Flight Activity.csv y Customer Loyalty History.csv en la misma raíz que el notebook.

Ejecución:
Ejecuta bbdd_flight_loyalty.ipynb de forma secuencial para reproducir los resultados y gráficos.
