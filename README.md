# Kaggle Competitions: Mi Camino en Data Science 🚀

Este repositorio es una bitácora de mi progreso en el mundo del Machine Learning y la Ciencia de Datos a través de retos de Kaggle. Aquí documento no solo el código final, sino la evolución de mis modelos, desde arquitecturas básicas hasta pipelines de producción robustos.

## 📌 Competencias Destacadas

### 🏠 House Prices - Advanced Regression Techniques
* **Objetivo:** Predecir el precio de venta de viviendas mediante técnicas de regresión avanzada.
* **Estatus:** Optimizado.

#### 📈 Evolución del Modelo
1.  **Iteración 1 (Base):** Uso de Random Forest con limpieza manual. Problemas detectados: Overfitting y falta de escalabilidad.
2.  **Iteración 2 (Pipelines):** Implementación de `Scikit-Learn Pipelines` y `ColumnTransformer`. Se automatizó el tratamiento de nulos y categorías, eliminando el "Data Leakage".
3.  **Iteración 3 (Lasso & Regularización):** Migración a modelos lineales regularizados (L1) para mejorar la generalización. 
4.  **Iteración 4 (Optimización Logarítmica):** Aplicación de transformación logarítmica (`log1p`) al target para corregir la heterocedasticidad.

* **Mejor Score en Kaggle:** 0.7562

---

## 🛠️ Stack Tecnológico y Metodología

Para asegurar que los modelos sean robustos y reproducibles, el flujo de trabajo incluye:

-   **Preprocesamiento:** Selección dinámica de columnas (numéricas/categóricas), imputación por mediana/moda y `OneHotEncoding` con manejo de categorías desconocidas.
-   **Modelado:** `GridSearchCV` para la búsqueda exhaustiva de hiperparámetros.
-   **Visualización:** Gráficos de residuos y dispersión (Real vs. Predicho) para detectar patrones de error.

---
