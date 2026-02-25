# 📡 TelecomX: Predicción de Fuga de Clientes (Churn)

Este proyecto forma parte del desafío de Ciencia de Datos enfocado en el sector de telecomunicaciones. El objetivo principal fue desarrollar un modelo de **Machine Learning** capaz de predecir qué clientes tienen mayor probabilidad de cancelar sus servicios, permitiendo a la empresa tomar acciones preventivas.

## 🚀 Resumen del Proyecto

A través de un análisis exhaustivo de los datos de **TelecomX**, se identificaron patrones de comportamiento que preceden a la cancelación del servicio. El proyecto abarca desde la limpieza de datos hasta la implementación de modelos predictivos de clasificación.

### 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python 3.x
* **Librerías:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn.
* **Técnicas:** SMOTE (Balanceo de clases), One-Hot Encoding, MinMaxScaler.

---

## 📊 Resultados del Modelo

Se compararon tres modelos de clasificación para encontrar el mejor predictor:

| Modelo | Precisión (Accuracy) |
| :--- | :---: |
| Dummy Classifier (Base) | 49.08% |
| K-Nearest Neighbors (KNN) | 79.72% |
| **Árbol de Decisión** | **79.57%** |

*Nota: Aunque KNN tuvo una ligera ventaja en precisión, el **Árbol de Decisión** fue seleccionado por su alta interpretabilidad para el negocio.*

---

## 💡 Hallazgos Críticos

El modelo identificó que la fuga de clientes no es aleatoria, sino que depende de factores específicos:

1.  **Tipo de Contrato:** Los contratos "Mes a Mes" son la principal fuente de riesgo. Los contratos anuales reducen significativamente la tasa de abandono.
2.  **Método de Pago:** Existe una alta correlación entre el uso de **Cheque Electrónico** y la cancelación del servicio.
3.  **Tecnología:** Los usuarios de **Fibra Óptica** con cargos elevados muestran una mayor sensibilidad y tendencia a la fuga.
4.  **Tenure (Antigüedad):** Los primeros 6 meses son críticos; la probabilidad de abandono disminuye drásticamente a medida que aumenta la antigüedad del cliente.

---

## 📈 Recomendaciones Estratégicas

* **Fidelización Contractual:** Incentivar la migración de contratos mensuales a anuales mediante beneficios en servicios de valor agregado.
* **Optimización de Pagos:** Promover el uso de métodos de pago automáticos para reducir la fricción mensual que genera el pago manual.
* **Atención Temprana:** Implementar campañas de retención específicas para clientes nuevos durante su primer semestre de permanencia.

---

## 📁 Estructura del Repositorio
* `TELECOM_X2.ipynb`: Cuaderno principal con el desarrollo del modelo (Etapa 2).
* `telecom_tratado.csv`: Dataset limpio y procesado utilizado para el entrenamiento.
* `README.md`: Descripción del proyecto y hallazgos.

---

**Desarrollado por:** Jorge Ramos 
**Fecha:** Febrero 2026
