# Análisis de Lealtad y Actividad de Vuelo ✈️

Este proyecto consiste en un análisis de datos integral de un programa de lealtad de una aerolínea. El objetivo es explorar el comportamiento de los clientes, limpiar anomalías en los datos y extraer información estadística relevante para la toma de decisiones estratégicas.

## 📋 Estructura del Proyecto

El análisis se divide en tres fases principales:

1. **Fase 1: Limpieza y Preparación de Datos**: 
   * Estandarización de nombres de columnas.
   * Tratamiento de valores nulos (especialmente en la columna `salary`).
   * Corrección de anomalías (conversión de salarios negativos).
   * Unión de los datasets de actividad de vuelo e historial de lealtad.

2. **Fase 2: Análisis Exploratorio de Datos (EDA)**:
   * Cálculo de estadísticas descriptivas (media, mediana, desviación estándar).
   * Identificación de valores atípicos (*outliers*) mediante el método del Rango Intercuartílico (IQR).
   * Análisis de correlación de Spearman para variables numéricas.

3. **Fase 3: Visualización**:
   * Creación de gráficos con Seaborn y Matplotlib para identificar patrones de comportamiento según estado civil, nivel educativo y tipo de tarjeta.

## 📊 Los Datasets

El proyecto utiliza dos archivos fuente:
* **Customer Flight Activity.csv**: Registros mensuales de vuelos reservados, distancia y puntos acumulados.
* **Customer Loyalty History.csv**: Perfil demográfico del cliente (salario, educación, ubicación, CLV).

## 🛠️ Tecnologías Utilizadas

* **Python 3.10+**
* **Pandas**: Manipulación y limpieza de datos.
* **NumPy**: Operaciones numéricas.
* **Seaborn & Matplotlib**: Visualización de datos.
* **Scikit-learn**: Imputación de valores nulos (`SimpleImputer`).

## 🚀 Cómo ejecutar el proyecto

1. Asegúrate de tener instaladas las librerías necesarias:

   pip install pandas numpy seaborn matplotlib scikit-learn

   Abre el archivo bbdd_flight_loyalty.ipynb en tu entorno de Jupyter Notebook o VS Code.

   Ejecuta las celdas en orden secuencial para reproducir la limpieza y el análisis.