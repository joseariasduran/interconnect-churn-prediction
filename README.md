# 📉 Predicción de Fuga de Clientes (Customer Churn) - Telecomunicaciones

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-LightGBM-orange)
![Status](https://img.shields.io/badge/Status-Completado-brightgreen)

## 📌 Resumen del Proyecto
Desarrollo de un modelo de Machine Learning predictivo para identificar a los clientes con alta probabilidad de cancelar sus servicios en **Interconnect**, un operador de telecomunicaciones. El objetivo es optimizar la asignación de presupuestos de retención (códigos promocionales y descuentos) dirigiéndolos exclusivamente a usuarios en riesgo real, maximizando el ROI de la campaña.

## 🎯 Objetivos Clave
* **Estrategia de Datos:** Unificar y limpiar 4 bases de datos relacionales (Contratos, Datos Personales, Servicios de Internet y Telefonía) mitigando valores nulos y errores de formato.
* **Métrica Objetivo:** Maximizar la métrica **AUC-ROC** para minimizar tanto los falsos positivos (promociones desperdiciadas) como los falsos negativos (fugas no detectadas).
* **Explicabilidad:** Identificar los factores comerciales exactos que impulsan la retención o el abandono del cliente.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn, LightGBM (Gradient Boosting)

## 📊 Resultados del Modelo
El modelo final basado en **LightGBM** (optimizando hiperparámetros y compensando el desbalance de clases) superó ampliamente la línea base de rendimiento:
* **AUC-ROC:** `0.88+` (Máximo estándar del proyecto alcanzado)
* **Exactitud (Accuracy):** `82%`

### 🔍 Hallazgos de Negocio (Feature Importance)
1. **Antigüedad vs. Volatilidad:** El tiempo de permanencia (`Tenure`) es el predictor más fuerte. La mayor tasa de fuga ocurre en los primeros 10 meses.
2. **Impacto Financiero:** Los clientes con el esquema de pago mensual y facturas por encima de la media presentan un riesgo crítico de abandono.
3. **Efecto de Retención:** Los servicios adicionales como *Soporte Técnico* y *Seguridad en Línea* actúan como un "blindaje", reduciendo drásticamente la probabilidad de fuga.

## 🚀 Cómo ejecutar este proyecto

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/interconnect-churn-prediction.git](https://github.com/tu-usuario/interconnect-churn-prediction.git)
