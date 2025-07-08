# 📊 Predicción de Cancelación de Clientes (Churn)

## 🧑‍💻 Autor 
**Nombre:** Alejandro Javier Contreras Olate

---

## 🎯 Descripción del Proyecto

Este proyecto aplica técnicas de ciencia de datos y machine learning para **predecir qué clientes están en riesgo de cancelar un servicio de telecomunicaciones**. Utiliza un enfoque progresivo en tres etapas: análisis exploratorio, modelado inicial y optimización avanzada.

El objetivo es desarrollar un modelo de machine learning capaz de:
- Detectar con alta precisión qué clientes están en riesgo de cancelar
- Ayudar al negocio a tomar **decisiones proactivas** para retener clientes
- Implementar un pipeline de trabajo replicable para problemas de churn

---

## 🚀 Dataset

 - Fuente: [Telco Customer Churn - Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
 - Archivo original: data/raw/WA_Fn-UseC_-Telco-Customer-Churn.csv
 - Archivo procesado: data/processed/telco_churn_featured.csv

---

## 🧠 Tecnologías Utilizadas

- **Python 3.10**
- **Jupyter Notebooks**
- **pandas, numpy, matplotlib, seaborn**
- **scikit-learn** (modelos base y métricas)
- **imbalanced-learn** (SMOTE)
- **XGBoost** (modelo optimizado)

---

## 🏗️ Estructura del Proyecto

```bash
Proyecto-Prediccion-de-Cancelacion-de-Clientes-Churn
├── data/
│   ├── processed/
│   │   └── telco_churn_featured.csv       # Datos procesados
│   └── raw/
│       └── WA_Fn-UseC_-Telco-Customer-Churn.csv  # Dataset original
├── notebooks/
│   ├── 01_EDA.ipynb                       # Exploración de datos
│   ├── 02_Modeling.ipynb                  # Modelos base: Logistic Regression, Random Forest
│   └── 03_OptimizacionAvanzada_SMOTE_XGBoost.ipynb  # SMOTE + XGBoost + métricas avanzadas
├── .gitignore                            # Ignora venv y archivos temporales
├── README.md                             # Documentación del proyecto
└── requirements.txt                      # Librerías necesarias
```

---

## 📁 Descripción de los Notebooks

### `01_EDA.ipynb`
- Limpieza de datos y detección de valores faltantes
- Análisis de distribución de variables numéricas y categóricas
- Visualización de correlaciones con la variable objetivo (Churn)
- Identificación de patrones relevantes

### `02_Modeling.ipynb`
- Codificación de variables categóricas
- División de datos en entrenamiento y prueba
- Entrenamiento de modelos base: Logistic Regression y Random Forest
- Evaluación con métricas: precisión, recall, F1, matriz de confusión

### `03_OptimizacionAvanzada_SMOTE_XGBoost.ipynb`
- Aplicación de SMOTE para balancear clases desbalanceadas
- Entrenamiento de un modelo avanzado con XGBoost
- Evaluación con curva ROC, AUC, y análisis de importancia de variables
- Comparación entre modelos

---

## ⚙️ Instalación

### 1. Clona este repositorio:
```bash
git clone https://github.com/Cotocross/Proyecto-Prediccion-de-Cancelacion-de-Clientes-Churn.git
cd proyecto-churn
```

### 2. Crea un entorno virtual (opcional pero recomendado):
```bash
python -m venv venv
venv\Scripts\activate     # Windows
source venv/bin/activate  # Mac/Linux
```

### 3. Instala las dependencias:
```bash
pip install -r requirements.txt
```

### 4. Ejecuta los notebooks con Jupyter o VS Code

---

## 📈 Resultados

- El modelo **XGBoost optimizado con SMOTE** logró un **AUC superior a 0.85**, mostrando un excelente poder predictivo
- Se identificaron variables críticas como el tipo de contrato, los cargos mensuales y la antigüedad del cliente
- Se generaron insights accionables para la retención de clientes

---

## 💼 Aplicación Empresarial

Este sistema de predicción permite a una empresa:

- **Detectar clientes en riesgo** antes de que cancelen
- **Aplicar campañas de retención** personalizadas
- **Aumentar el ingreso promedio** por cliente (ARPU)
- **Reducir los costos de adquisición** de nuevos clientes

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - consulta el archivo [LICENSE](LICENSE) para más detalles.

---



