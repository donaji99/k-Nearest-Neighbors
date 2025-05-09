# K-Nearest Neighbors (KNN) para Detección de Fraude Financiero 💳

Este proyecto aplica el algoritmo de **K Vecinos más Cercanos (KNN)** a una base de datos de transacciones financieras con el objetivo de **detectar fraudes**. El análisis fue realizado en Jupyter Notebook como parte de una práctica académica y también para enriquecer mi portafolio profesional de Ciencia de Datos.

---

## 🔗 Fuente de los Datos

- Dataset: [Synthetic Financial Dataset For Fraud Detection](https://www.kaggle.com/datasets/ealaxi/paysim1)
- Contiene transacciones financieras simuladas, categorizadas como fraude o no fraude.
- Variable objetivo: `isFraud` (1 = fraude, 0 = legítima)

---

## 📊 Variables Seleccionadas

Se utilizaron las siguientes variables descriptivas:

- `amount`: Monto de la transacción.
- `oldbalanceOrg`: Balance del remitente antes de la transacción.
- `newbalanceOrig`: Balance del remitente después de la transacción.
- `oldbalanceDest`: Balance del destinatario antes de la transacción.
- `newbalanceDest`: Balance del destinatario después de la transacción.

---

## 📈 Proceso

1. **Preprocesamiento**:
   - Se realizó muestreo estratificado para evitar desbalance extremo en las clases.
   - Se aplicó escalado (`StandardScaler`) a las variables para mejorar el desempeño del algoritmo KNN.

2. **Modelado**:
   - Se entrenaron múltiples modelos de KNN con distintos pares de variables.
   - Finalmente, se entrenó un modelo con todas las variables descriptivas.

3. **Evaluación**:
   - Se evaluó el rendimiento con la métrica de **accuracy**.
   - El modelo final alcanzó una **exactitud de 0.9994**.

---

## 🧠 Lecciones Aprendidas

- KNN puede ser muy efectivo para tareas de clasificación binaria cuando se realiza un buen preprocesamiento.
- El escalado de variables es crítico para evitar tiempos de ejecución prolongados y mejorar precisión.
- Detectar fraudes a partir de patrones numéricos es una tarea donde los algoritmos supervisados pueden destacar.

---

## ⚙️ Tecnologías Usadas

- Python
- Jupyter Notebook
- Pandas, NumPy
- Scikit-learn (KNN, StandardScaler, train_test_split)
- Matplotlib y Seaborn

---

## ✍️ Autor

Donají Ramos Núñez – [Portafolio en GitHub](https://github.com/tu-usuario)  
Maestría en Ciencia de Datos – Universidad Tecnológica de la Mixteca  
