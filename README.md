# 📊 Breast Cancer Wisconsin (Diagnostic) – EDA

## 🎯 Objetivo del proyecto
El objetivo de este trabajo es realizar un análisis exploratorio de datos (EDA) completo sobre un dataset real, siguiendo un flujo ordenado de carga, exploración, limpieza y visualización.

---

## 1. Descripción del dataset
Este EDA se ha realizado sobre el **Breast Cancer Wisconsin (Diagnostic) Dataset**, bastante utilizado para el análisis de características morfológicas de tumores benignos y malignos a partir de biopsias FNA (Fine Needle Aspiration).  

El dataset original proviene del repositorio de **UCI Machine Learning Repository**.

---

## 2. Contenido del análisis

### Carga y exploración inicial  
- Visualización de dimensiones, columnas y tipos de datos.  
- Inspección de valores nulos, duplicados y rangos con `describe()`.  
- Análisis de la calidad del dataset y su granularidad.

### Limpieza aplicada  
- Eliminación de la columna `Unnamed: 32` por estar completamente vacía.  
- Conversión de `diagnosis` al tipo **categoría**.  
- Revisión y decisión sobre el uso de `id` como identificador.  
- Confirmación de ausencia de duplicados y nulos tras la limpieza.

### Visualizaciones realizadas  
- Histograma de una variable numérica relevante.  
- Gráfica de barras de la variable objetivo (`diagnosis`).  
- Mapa de calor de correlación entre variables numéricas.

### Conclusiones principales  
- El dataset está desbalanceado a favor de casos benignos.  
- Las variables relacionadas con el tamaño del tumor (`radius`, `perimeter`, `area`) muestran altas correlaciones.  
- Las métricas con sufijo *worst* parecen más representativas en el diagnóstico.  
- El dataset quedó limpio y preparado para un análisis o modelado posterior.

---

## 3. Fuente del dataset  
Dataset original:  
UCI Machine Learning Repository – Breast Cancer Wisconsin (Diagnostic)
[Enlace de kaggle](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data/data)

---

## 4. Reflexión personal
Al analizar este dataset, me ha llamado especialmente la atención cómo ciertas características de los tumores están claramente asociadas a que el diagnóstico sea maligno. Variables como el radio, el perímetro y el área muestran valores significativamente más altos en los casos malignos, y esto es especialmente evidente en las mediciones etiquetadas como worst, que representan las peores observaciones de cada tumor.

Aunque se trata de datos puramente biomédicos, tienen una dimensión humana evidente. En mi caso, este análisis me tocaba de cerca porque mi abuela superó un cáncer de mama. Ver cómo los datos reflejan el comportamiento real de los tumores malignos me ha ayudado a entender mejor cómo los médicos valoran estas señales.
