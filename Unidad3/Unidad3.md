# 🤖 Unidad 3: Modelos Probabilísticos y Regresión

## 📁 Contenedor de Entregas Finales

Este directorio agrupa las herramientas analíticas dedicadas al modelado predictivo y la evaluación de variables de respuesta continuas y categóricas:

1. **Cuadernos Experimentales (APE11 a APE16):** Laboratorios interactivos para el desarrollo de modelos de regresión, análisis de correlación y evaluación de clasificadores.
2. **Data Source (`data_source/`):** Archivo base de la Encuesta Nacional de Empleo, Desempleo y Subempleo (ENEMDU), módulo de Vivienda y Hogar (periodo 2026-02).

---

## 🗺️ 1. Estructura de Actividades Prácticas Experimentales (Laboratorios)

Haga clic en cualquiera de los enlaces para revisar la documentación, el código y la resolución técnica interactiva:

* [📊 Laboratorio APE11: Inferencia Estadística Multigrupo (ANOVA de 1 Factor) y Pruebas Post-Hoc (Tukey)](./APE/APE11_InferenciaEstadistica_GrupoE.ipynb)
  
  *Segmentación de hogares según tipo de vivienda y análisis de varianza del gasto en arriendo, incluyendo validación de supuestos (Levene) y prueba alternativa no paramétrica de Kruskal-Wallis.*

* [📈 Laboratorio APE12: Análisis Bivariado y Predicción: Correlación de Pearson y Modelo de Regresión Lineal Simple (OLS)](./APE/APE_012_AnalisisBivariado.ipynb)
  
  *Estudio de la relación lineal entre el número de cuartos y el valor del arriendo, cálculo del coeficiente de correlación, ajuste del modelo OLS y generación de predicciones puntuales con extrapolación.*

* [📉 Laboratorio APE13: Regresión Lineal Múltiple: Modelado Multivariado y Diagnóstico de Multicolinealidad (VIF)](./APE/APE_014_RegresionMultiple.ipynb)
  
  *Construcción de un modelo predictivo multivariado, análisis de correlación mediante pairplot y heatmap, y detección de multicolinealidad mediante el Factor de Inflación de la Varianza (VIF).*

* [📋 Laboratorio APE14: Regresión Logística: Modelado de Probabilidades y Matriz de Confusión](./APE/APE_015_Logistica.ipynb)
  
  *Aplicación de la función sigmoide para la clasificación binaria, ajuste del modelo Logit, evaluación de la matriz de confusión y análisis del impacto del umbral de decisión (Thresholding) en el balance de errores.*

* [🏆 Laboratorio APE15: Evaluación Avanzada de Modelos: Curva ROC, AUC y Validación Cruzada (K-Fold)](./APE/APE_016_ValidacionROC.ipynb)
  
  *Evaluación de la capacidad discriminante de un modelo de regresión logística mediante la Curva ROC y el Área Bajo la Curva (AUC), consolidación del modelo regional del Proyecto Integrador y análisis de robustez mediante validación cruzada estocástica (K-Fold).*

---

## 📓 3. Resumen de Autoevaluación y Aprendizaje

### 🔬 Conceptos Clave Asimilados

Durante la Unidad 3, se consolidaron los fundamentos del modelado predictivo, evolucionando desde el análisis de relaciones bivariadas (Correlación de Pearson) hacia la construcción de modelos de regresión lineal y logística. Se comprendió la importancia de la significancia estadística de los coeficientes (valor-p) y la interpretación de métricas de ajuste como el **R²** en regresión y la **Exactitud** y **Sensibilidad** en clasificación.

Se aplicaron técnicas de diagnóstico de modelos, como el análisis de multicolinealidad mediante el **Factor de Inflación de la Varianza (VIF)** y la evaluación del rendimiento a través de la **Curva ROC** y el **AUC**, entendiendo la diferencia entre una métrica dependiente de un umbral (exactitud) y una métrica independiente del mismo (AUC).

Se exploró el concepto de **Validación Cruzada Estocástica (K-Fold)** para obtener estimaciones más robustas del rendimiento del modelo y cuantificar su estabilidad, reconociendo las limitaciones de evaluar un modelo con una sola partición de datos. Se reforzó el uso de librerías como `scikit-learn` y `statsmodels` para la implementación de estos modelos y técnicas de evaluación.

### ⚠️ Retos de Programación Superados

Uno de los principales retos fue la correcta preparación de los datos para el modelado, incluyendo la codificación de variables categóricas (*one-hot encoding*) para la regresión logística y la verificación de supuestos como la homocedasticidad en modelos lineales. Se superaron dificultades en la interpretación de la salida de `statsmodels` para modelos logísticos y en la implementación de la validación cruzada con `cross_val_score`.

Otro desafío significativo fue el ajuste y la interpretación del umbral de decisión (threshold) en clasificación, entendiendo el *trade-off* entre **Falsos Positivos** y **Falsos Negativos** y su impacto en la toma de decisiones. Se desarrolló la habilidad de traducir los resultados de las métricas de evaluación (como el AUC y la matriz de confusión) en conclusiones prácticas para un problema de negocio regional.

### 📌 Conclusión General

La Unidad 3 integró los conocimientos de probabilidad e inferencia estadística para la creación de modelos predictivos útiles en la toma de decisiones. Se aplicaron técnicas de regresión lineal y logística a datos reales de la ENEMDU para predecir variables de interés como el arriendo y el acceso a servicios básicos.

El uso de Python y sus librerías especializadas permitió automatizar el proceso de modelado, desde la limpieza y preparación de datos hasta la evaluación y validación de modelos, demostrando la potencia de la computación para el análisis de datos y la solución de problemas prácticos en contextos como la planificación de infraestructura pública y el análisis socioeconómico. Este proceso fortaleció las competencias en programación, estadística aplicada y comunicación de resultados.
