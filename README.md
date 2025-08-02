# 🧬 Breast Cancer Classification

Este proyecto aplica algoritmos de Machine Learning para predecir si una muestra de tejido mamario es **benigna** o **maligna**, utilizando el dataset de Breast Cancer Wisconsin. Se entrenaron y compararon tres modelos de clasificación supervisada con especial atención a la métrica **balanced accuracy**, adecuada en escenarios con posible desbalance de clases.

---

## 📂 Dataset

- **Variable objetivo:** Clasificación del tumor (2: benigno, 4: maligno)

---

## ⚙️ Modelos utilizados

- 🔵 Regresión Logística
- 🟢 Support Vector Machine (SVM) lineal
- 🔴 Random Forest

Cada modelo fue evaluado con **validación cruzada 10-fold** utilizando la métrica **balanced accuracy** para asegurar una evaluación equilibrada entre clases.

---

## 📊 Resultados

| Modelo              | Balanced Accuracy |
|---------------------|-------------------|
| Regresión Logística | 0.97              |
| SVM lineal          | 0.97              |
| Random Forest       | 0.95              |

> 🔎 Regresión Logística y SVM lineal obtuvieron el mejor desempeño. Esta coincidencia se debe a que ambos son clasificadores lineales y el dataset presenta una clara separación entre clases. Random Forest no superó a los modelos lineales, posiblemente por una leve sobreajuste o por la ausencia de relaciones no lineales fuertes.

---


## 📈 Visualización de rendimiento

### 📊 Balanced Accuracy por Modelo

El gráfico a continuación muestra la distribución real de los valores de balanced accuracy obtenidos en validación cruzada para cada modelo. Se visualizan mediante boxplots acompañados de los puntos individuales de cada fold.

Esto permite comparar tanto el rendimiento promedio como la estabilidad de cada clasificador.

![Boxplot de Balanced Accuracy](imagen1.png)

---

## 📌 Conclusiones

- Los tres modelos presentan un **rendimiento elevado y consistente**, con valores de balanced accuracy superiores al 90%.
- **Regresión Logística** y **SVM lineal** obtuvieron el **mayor rendimiento promedio (0.97)** y además una **variabilidad muy baja**, lo que sugiere que son modelos estables y confiables.
- **Random Forest**, si bien alcanzó un rendimiento competitivo (0.95), mostró una **ligeramente mayor dispersión** en sus resultados, posiblemente debido a su complejidad y sensibilidad a los datos de entrenamiento.
- El uso de **boxplots con puntos reales** permite una evaluación más completa que solo el promedio, ya que revela la **robustez de cada modelo frente a diferentes particiones de datos**.

---

## ✅ Recomendaciones

- Priorizar modelos como **Regresión Logística** o **SVM lineal** para este tipo de problema, ya que combinan **precisión, estabilidad e interpretabilidad**.
- Utilizar siempre **validación cruzada** y métricas como balanced accuracy, especialmente cuando las clases están desbalanceadas.
- Incorporar análisis de **matriz de confusión**, **precision**, **recall** y **F1-score** para una evaluación más profunda del comportamiento del modelo.
- Realizar análisis de **importancia de variables** o aplicar técnicas de **reducción de dimensionalidad** para mejorar la interpretabilidad sin perder rendimiento.
- Visualizar no solo el promedio, sino también la **variabilidad del modelo** para tomar decisiones más robustas.


---

## 🚀 Autor

**Diego Arroyo**  
📧 diegojulioarroyo@gmail.com  
🔗 [Mi LinkedIn](https://www.linkedin.com/in/diego-arroyo-b2153b229/) 
