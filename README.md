# sprint7-final-project
Proyecto de analisis de datos
# Análisis de Segmentación de Clientes - ConnectaTel

Este proyecto realiza un análisis exploratorio de datos (EDA) y una segmentación estratégica de la base de clientes de **ConnectaTel**. El objetivo es identificar patrones de consumo, clasificar a los usuarios según su comportamiento y demografía, y proponer recomendaciones comerciales accionables para la toma de decisiones.

---

## 🎯 Objetivo del Proyecto

El propósito principal de este análisis es:
1. **Limpiar y validar** la consistencia de los datos de consumo de los clientes.
2. **Segmentar a los usuarios** en categorías basadas en su nivel de uso (llamadas y mensajes) y su edad.
3. **Analizar patrones extremos (outliers)** para evaluar su impacto en el negocio.
4. **Generar insights ejecutivos** que permitan a los tomadores de decisiones diseñar planes de telefonía más eficientes y personalizados.

---

## 📊 Datasets Utilizados

El análisis se basa en el dataset de perfiles de usuario de ConnectaTel:
* **`user_profile`**: Contiene información de 4,000 usuarios con las siguientes variables clave:
  * `age`: Edad del usuario.
  * `cant_mensajes`: Cantidad de mensajes de texto enviados en el periodo.
  * `cant_llamadas`: Cantidad de llamadas telefónicas realizadas.
  * `cant_minutos_llamada`: Duración total de las llamadas en minutos.

---

## 📈 Etapas del Análisis Realizadas

El proyecto se estructuró en las siguientes fases metodológicas:

1. **Exploración Inicial**: Carga del dataset, análisis de tipos de datos, estadísticas descriptivas y detección de valores nulos o inconsistentes.
2. **Tratamiento de Outliers**: Evaluación de los límites superiores mediante el método de Rango Intercuartílico (IQR). Decisión justificada de mantener los valores atípicos para el análisis de *Heavy Users*.
3. **Ingeniería de Características (Segmentación)**:
   * Creación de la columna `grupo_uso` (Bajo uso, Uso medio, Alto uso).
   * Creación de la columna `grupo_edad` (Joven, Adulto, Adulto Mayor).
4. **Visualización de Datos**: Creación de gráficos de barras (`countplot` con Seaborn) para analizar la distribución de los segmentos.
5. **Generación de Insights y Recomendaciones**: Redacción de conclusiones de negocio basadas en los hallazgos demográficos y de consumo.

---

## 🚀 Cómo Ejecutar el Notebook

Puedes visualizar y ejecutar este proyecto de forma interactiva de dos maneras:

### Opción 1: En Google Colab (Recomendado)
1. Ve a [Google Colab](https://colab.research.google.com/).
2. Selecciona la pestaña **GitHub**.
3. Pega la URL de este repositorio y selecciona el archivo `.ipynb`.
4. Ejecuta las celdas en orden presionando `Shift + Enter`.

### Opción 2: Localmente (Jupyter Notebook)
Si prefieres correrlo en tu computadora, asegúrate de tener instalado Python y Jupyter:
1. Clona este repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/nombre-del-repositorio.git](https://github.com/tu-usuario/nombre-del-repositorio.git)
