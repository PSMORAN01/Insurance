# Predicción de beneficios de seguro médico 🩺📈

Este proyecto tiene como objetivo analizar un conjunto de datos de clientes y predecir el número de beneficios de seguro médico que podrían recibir, utilizando modelos de regresión y algoritmos de vecinos más cercanos (KNN). Se exploran también los efectos del escalado y distintas métricas de distancia sobre el desempeño del modelo.

---

## 📊 Descripción general

Se utilizó un dataset llamado `insurance_us.csv` con las siguientes columnas relevantes:

- `gender` — género del cliente
- `age` — edad
- `income` — ingreso anual
- `family_members` — cantidad de familiares
- `insurance_benefits` — número de beneficios de seguro recibidos

El objetivo fue predecir el valor de `insurance_benefits` a partir de las otras características, usando enfoques supervisados y análisis de similitud.

---

## ⚙️ Tecnologías utilizadas

- Python 3
- Pandas
- NumPy
- Seaborn
- Scikit-learn (LinearRegression, NearestNeighbors, escaladores, métricas)

---

## 🧪 Procesamiento y modelado

1. **Preprocesamiento:**
   - Renombrado de columnas
   - Conversión de tipos (por ejemplo, `age` a entero)
   - Escalado de características con `MaxAbsScaler`

2. **Análisis exploratorio:**
   - Estadísticas descriptivas
   - Gráficos de correlación y distribución (usando `pairplot` de Seaborn)

3. **Modelado:**
   - Regresión lineal simple (`LinearRegression`)
   - Algoritmo de vecinos más cercanos (`KNN`) usando `NearestNeighbors`
   - Comparación con y sin escalado
   - Evaluación con métricas como RMSE y R²

---

## 📈 Resultados

- El escalado de los datos tuvo un impacto positivo al aplicar KNN, mejorando la comparación entre clientes.
- El modelo fue capaz de identificar clientes similares en términos de edad, ingresos y tamaño familiar.
- Se construyó una función `get_knn()` para obtener vecinos más cercanos personalizados, probando distintas métricas (euclidiana, manhattan, etc.).

---

## 🧠 Lecciones aprendidas

- Escalar los datos antes de aplicar algoritmos basados en distancia es fundamental.
- La regresión lineal ofrece una buena línea base, pero modelos basados en similitud pueden ser más interpretables en este tipo de contextos.
- La creación de funciones personalizadas como `get_knn()` ayuda a profundizar en el comportamiento del modelo y explorar la lógica detrás de las recomendaciones.

---

## 👨‍💻 Autor

**Pablo Sebastián Morán**  
📧 psmoran01@gmail.com  
🔗 [GitHub](https://github.com/PSMORAN01)  
