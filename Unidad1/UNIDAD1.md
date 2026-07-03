# 📈 Unidad 1: Fundamentos de Probabilidad y Distribuciones
## 📁 Organización de Archivos
Este espacio contiene los cuadernos de código correspondientes a las primeras semanas de experimentación:
1. **Modelos Algorítmicos (APE00 a APE05):** Cuadernos `.ipynb` con simulaciones, álgebra de eventos y análisis de forma de variables aleatorias.

---

## 🗺️ 1. Estructura de Actividades Prácticas Experimentales (Laboratorios)
Haga clic en cualquiera de las guías para revisar la documentación y resolución técnica original de la Unidad 1:

* [📄 Laboratorio APE00: Fundamentos de Probabilidad y Espacios Muestrales](./APE/APE00.ipynb)  
  *Simulación en Python de fenómenos aleatorios mediante la definición analítica de espacios muestrales y eventos probabilísticos.*
* [📄 Laboratorio APE01: Variables Aleatorias y Distribuciones de Probabilidad](./APE/APE01.ipynb)  
  *Implementación algorítmica para evaluar el comportamiento intrínseco de variables aleatorias mediante funciones de masa y densidad.*
* [📄 Laboratorio APE02: Distribuciones Muestrales y Teorema del Límite Central](./APE/APE02.ipynb)  
  *Validación experimental del comportamiento del promedio de las muestras y su aproximación continua a la normalidad.*
* [📄 Laboratorio APE03: Variables Aleatorias Discretas y Continuas](./APE/APE03.ipynb)  
  *Evaluación de funciones continuas mediante aproximaciones numéricas frente al mapeo discreto en conjuntos de datos.*
* [📄 Laboratorio APE04: Momentos Estadísticos y Análisis de Tendencia Central con Python](./APE/APE04.ipynb)  
  *Programación de scripts para calcular la Esperanza $E[X]$, la Varianza $V[X]$ y estimadores de asimetría sobre colecciones de datos.*
* [📄 Laboratorio APE05: Distribuciones Discretas Notables](./APE/APE05.ipynb)  
  *Uso interactivo de distribuciones de Poisson y Binomial mediante `scipy.stats` para resolver problemas basados en escenarios prácticos.*

---

## 📓 2. Resumen de Autoevaluación y Aprendizaje

### 🔬 Conceptos Clave Asimilados
* **Manejo Descriptivo Integral:** Comprensión de cómo las métricas de tendencia central (media y mediana) se complementan con los índices de dispersión (varianza y desviación) para estructurar un resumen analítico completo.
* **Aplicación de Teoremas Estocásticos:** Diseño algorítmico de experimentos para comprobar la probabilidad condicional y resolver problemas complejos mediante la actualización de datos condicionados por el Teorema de Bayes.
* **Morfología de Variables Probabilísticas:** Diferenciación operativa de variables continuas y discretas mediante la codificación de funciones de masa (PMF), densidad (PDF) y distribución acumulada (CDF), ligadas a sus momentos analíticos de primer y segundo orden.

### ⚠️ Retos de Programación Superados
* **Ajuste y Calce de Gráficos:** Lograr superponer de manera exacta una curva de densidad teórica continua sobre un histograma empírico discontinuo fue una dificultad compleja. Se requirió forzar al entorno gráfico a normalizar el área total de las barras usando `density=True`.
* **Abstracción Analítica:** Cambiar el enfoque mental de calcular probabilidades directas por el de calcular áreas bajo la curva (integración) al pasar del contexto discreto al continuo.

### 📌 Conclusión General
El bloque inicial funcionó como una base para conectar las reglas puras del azar con scripts funcionales, demostrando que la estadística moderna requiere obligatoriamente del soporte computacional para ser modelada eficazmente.
