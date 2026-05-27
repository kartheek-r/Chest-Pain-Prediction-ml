# 🫀 Chest Pain Prediction using Machine Learning

> A machine learning project that predicts **musculoskeletal chest pain severity** based on mental health and lifestyle factors such as anxiety, depression, stress, sleep, and physical activity.

---

## 📌 Project Overview

Chest pain is often associated with heart disease — but a significant portion of chest pain cases are **musculoskeletal**, driven by psychological and lifestyle factors. This project builds a classification model to predict the **pain level** of a patient using mental health indicators, helping prioritize care and early intervention.

---

## 🎯 Objective

To analyze how psychological and lifestyle factors (anxiety, depression, stress, sleep, physical activity) influence musculoskeletal chest pain and build a predictive ML model to classify pain severity.

---

## 📂 Project Structure

```
Chest-Pain-Prediction-ml/
│
├── chest_pain_prediction_ml.ipynb    # Full ML pipeline (EDA → Model → Evaluation)
├── anxiety_depression_data.csv       # Dataset (Kaggle)
└── README.md
```

---

## 🗂️ Dataset Description

**Source:** Kaggle

| Feature | Description |
|---------|-------------|
| `Anxiety Score` | Patient's anxiety level score |
| `Depression Score` | Patient's depression level score |
| `Stress Level` | Self-reported stress level |
| `Sleep Hours` | Average hours of sleep per night |
| `Physical Activity` | Frequency of physical activity |
| `Pain_Level` | Target variable (engineered — Low / Medium / High) |

> **Note:** The `Pain_Level` target column was **feature engineered** from the raw data to create a meaningful classification label.

---

## 🛠️ Tools & Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

---

## ⚙️ ML Pipeline

### 1. 🧹 Data Preprocessing
- Loaded and inspected the dataset for null values and data types
- Handled missing values and inconsistent entries
- Scaled/normalized features for model compatibility

### 2. 🔧 Feature Engineering
- Created the target variable `Pain_Level` (Low / Medium / High) from raw data
- Selected relevant features: Anxiety Score, Depression Score, Stress Level, Sleep Hours, Physical Activity

### 3. 📊 Exploratory Data Analysis (EDA)
- Distribution plots for each feature
- Correlation heatmap to identify relationships between mental health factors and pain
- Analysis of how stress and anxiety relate to pain severity

### 4. 🤖 Model Building
- **Algorithm:** Random Forest Classifier
- Train/Test split for model evaluation
- Hyperparameter tuning for improved performance

### 5. 📈 Model Evaluation
- **Accuracy: ~65–70%**
- Confusion Matrix analysis
- Classification report (Precision, Recall, F1-Score)

---

## 💡 Key Insights

- 😰 **High anxiety and stress** are the strongest predictors of elevated chest pain levels
- 😴 **Poor sleep** (< 6 hours) correlates significantly with higher pain scores
- 🏃 **Regular physical activity** is associated with lower pain levels
- 😔 **Depression score** alone is a moderate predictor but amplifies effects of other factors
- ✅ The model successfully distinguishes between Low and High pain levels

---

## 🔮 Future Scope

- Integrate real-time health monitoring data (wearables)
- Deploy as a **Streamlit web app** for patient self-assessment
- Explore deep learning models (Neural Networks) for improved accuracy
- Expand dataset with more demographic features
- Build a mobile app for healthcare providers

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/kartheek-r/Chest-Pain-Prediction-ml.git
cd Chest-Pain-Prediction-ml

# 2. Install dependencies
pip install pandas scikit-learn matplotlib seaborn jupyter

# 3. Launch the notebook
jupyter notebook chest_pain_prediction_ml.ipynb
```

---

## 📊 Results Summary

| Metric | Value |
|--------|-------|
| Algorithm | Random Forest Classifier |
| Accuracy | ~65–70% |
| Target Classes | Low / Medium / High Pain |
| Key Features | Anxiety Score, Stress Level, Sleep Hours |

---

## 🙌 Conclusion

This project demonstrates the application of machine learning in the **healthcare domain** to predict pain levels based on mental health data. It highlights the strong connection between psychological well-being and physical pain, and shows how data-driven models can support early clinical decisions.

---

## 👨‍💻 Author

**Ryalampadu Kartheek**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kartheek-ryalampadu)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:kartheekryalampadu@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/kartheek-r)
