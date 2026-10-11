# ☀️ Solar Panel Recommendation ML

A machine learning project that classifies household **solar-investment likelihood**
as Low, Moderate, or High using synthetic household energy and financial data.

---

## 📊 Dataset

The project uses the **PowerPulse Synthetic Energy Insights Dataset**
with **100,000 records**.

Key features include:

- Monthly Income
- Energy Consumption
- Energy Cost
- CO₂ Emissions
- Solar Energy Generation
- Appliance Usage
- Region and Weather

The target, `buy_decision`, was engineered using financial,
energy-consumption, and environmental factors.

---

## 🤖 Machine Learning

Four classification models were evaluated:

- Support Vector Machine (SVM)
- Naive Bayes
- Random Forest
- Multilayer Perceptron (MLP)

The workflow included:

**EDA → Feature Engineering → Scaling → Model Training → GridSearchCV → Evaluation**

Both **StandardScaler** and **QuantileTransformer** were explored.

---

## 📈 Reported Results

| Model | Initial Test Accuracy | Tuned Test Accuracy |
|---|---:|---:|
| SVM | 65.25% | 67.75% |
| Naive Bayes | 68.13% | 67.00% |
| MLP | 50.88% | 67.31% |
| Random Forest | 68.63% | **68.81%** |

The experiments show the largest improvement for the MLP after preprocessing
and hyperparameter tuning, while Random Forest achieved the highest reported
test accuracy.

---

## 🛠️ Technologies

- Python
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn
- GridSearchCV
- Streamlit
- Pickle

---

## 🌐 Deployment

A Streamlit prototype was developed to provide solar-investment recommendations
based on household inputs such as income, energy consumption, and CO₂ emissions.

---

Academic team project – Princess Nourah bint Abdulrahman University
