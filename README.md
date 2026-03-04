# Predicción de Abandono de Clientes (Churn Analysis) 📊
Este proyecto implementa un flujo de ciencia de datos para identificar clientes en riesgo de cancelar sus servicios, comparando modelos de Regresión Logística y Random Forest.

# 🚀 Instalación y Preparación

Al ser un proyecto desarrollado en Google Colab, no requiere una instalación local compleja. Sigue estos pasos:

1. Carga del Notebook: Abre el archivo .ipynb en Google Colab.

2. Carga de Datos: El proyecto requiere un archivo externo llamado datos_tratados.csv.

    * Ve al icono de carpeta en la barra lateral izquierda de Colab.

    * Arrastra y suelta tu archivo .csv allí.

3. Librerías Necesarias: El entorno de Colab ya incluye la mayoría, pero si ejecutas de forma local, asegúrate de tener:

* pandas

* numpy

* matplotlib

* seaborn

* scikit-learn


# 🛠️ DependenciasEl 
proyecto utiliza las siguientes herramientas principales:
  * **Manipulación de datos:** Pandas y NumPy.
  * **Visualización:** Matplotlib y Seaborn.
  * **Machine Learning:** Scikit-Learn (específicamente LogisticRegression, RandomForestClassifier y LabelEncoder).
  * **Selección de características:** Test estadístico Qui-cuadrado ($\chi^2$).

# 🏃 **Cómo Ejecutar el Proyecto**
**Limpieza y Selección:** Ejecuta las celdas iniciales para procesar los datos y filtrar variables mediante el test de Qui-cuadrado ($p-value < 0.05$).

**Entrenamiento:** El notebook entrenará automáticamente dos modelos:
* Regresión Logística: Como modelo base de interpretación lineal.
* Random Forest: Con ajuste de pesos balanceados para mejorar la detección.
    
**Evaluación:** Al final, se generará una comparativa de matrices de confusión para decidir el mejor modelo.

# 📈 Resultados Clave
**Modelo Ganador:** El modelo de **Random Forest** es el recomendado para el negocio, ya que maximiza la captura de clientes en riesgo, permitiendo acciones de retención oportunas.

**Capacidad de Detección:** 74% de los clientes en riesgo (Recall).

**Variables más influyentes:** Antigüedad (Tenure), Cargos Mensuales y Tipo de Contrato.
