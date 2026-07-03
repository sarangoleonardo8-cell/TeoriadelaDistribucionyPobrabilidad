# 📊 Unidad 2: Inferencia Estadística y Pruebas de Hipótesis
## 📁 Contenedor de Entregas Finales
Este directorio almacena las herramientas analíticas dedicadas al modelamiento paramétrico y contraste de datos reales:
1. **Cuadernos Experimentales (APE06 a APE10):** Laboratorios interactivos aplicados a la inferencia.
2. **Evaluación de Cierre de Unidad:** Archivo principal del examen de código (`Jefferson_Sarango_Examen_U2.ipynb`).
3. **Data Source (`data_source/`):** Archivo maestro con las remuneraciones del GAD Municipal de Loja.

---

## 🗺️ 1. Estructura de Actividades Prácticas Experimentales (Laboratorios)
Haga clic en cualquiera de los enlaces para revisar la documentación, el código y la resolución técnica interactiva:

* [📄 Laboratorio APE06: Distribuciones Continuas Notables](./APEs/APE06.ipynb)  
  *Modelamiento de la campana de Gauss, estandarización de variables y aplicación práctica de la tabla Z mediante software.*
* [📄 Laboratorio APE07: Distribuciones Muestrales y Teorema del Límite Central (TLC) mediante Simulación Estocástica](./APEs/APE07.ipynb)  
  *Generación masiva de muestras por simulación para demostrar visual y matemáticamente el cumplimiento asintótico del TLC.*
* [📄 Laboratorio APE08: Inferencia Estadística: Estimación de Parámetros e Intervalos de Confianza (Z y T de Student)](./APEs/APE08.ipynb)  
  *Cálculo automatizado de intervalos de confianza para predecir medias bajo varianzas poblacionales conocidas y desconocidas.*
* [📄 Laboratorio APE09: Inferencia Estadística: Pruebas de Hipótesis Paramétricas (Z y T) y Análisis del Valor-p](./APEs/APE09.ipynb)  
  *Ejecución de contrastes empíricos de hipótesis paramétricas e interpretación crítica del valor-$p$ como regla para rechazar la hipótesis nula.*
* [📄 Laboratorio APE10: Inferencia Estadística Multigrupo: Análisis de Varianza (ANOVA de 1 factor) y Pruebas Post-Hoc (Tukey)](./APEs/APE10.ipynb)  
  *Implementación de contrastes de varianza multilinea y comparación simultánea por parejas para mitigar la inflación del error Tipo I.*

---

## 📓 2. Resumen de Autoevaluación y Aprendizaje

### 🔬 Conceptos Clave Asimilados
* **Inferencia y Métodos Estimativos:** Uso práctico de las distribuciones normal $Z$ y $T$ de Student para generar intervalos de confianza realistas sobre parámetros muestrales.
* **Validación de Supuestos a través del Valor-$p$:** Dominio de la librería `scipy.stats` para estructurar hipótesis de investigación y evaluar la significancia estadística frente a un nivel de alfa prefijado ($\alpha = 0.05$).
* **Modelos Multigrupo y Control de Error:** Aplicación de modelos lineales OLS en `statsmodels` para realizar análisis ANOVA de una vía, complementado con el algoritmo de Tukey HSD para aislar las variaciones estadísticas significativas bajo el parámetro visual `reject = True`.

### ⚠️ Retos de Programación Superados
1. **Limpieza de Formatos Gubernamentales Inconsistentes:** El archivo original de Loja contenía anomalías de codificación y strings corruptos con espacios al final de las celdas. Se corrigió usando la función vectorizada `df.columns.str.strip()` para limpiar los nombres de las variables y que el motor `openpyxl` pudiera operar el modelo lineal.
2. **Paradoja de Muestras de Gran Volumen:** Comprender que al trabajar con bases masivas ($N = 2883$), el error estándar se reduce tanto que los estadísticos de prueba ($t$ y $F$) crecen a niveles enormes, provocando que los valores-$p$ den potencias científicas diminutas (`e-236`). Aprendí que esto representa un poder de resolución prácticamente absoluto debido al tamaño de la muestra.

### 📌 Conclusión General
Esta unidad reafirmó la importancia de las ciencias de la computación como aliadas de la estadística inferencial. Automatizar estas pruebas paramétricas demuestra que el código es fundamental para realizar auditorías transparentes y extraer patrones de información real a partir de datos administrativos públicos.
