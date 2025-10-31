# 🩺 Heart Disease Prediction using Logistic Regression & Feature Engineering  

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Data%20Visualization-teal?logo=seaborn)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📖 Project Overview  
This project focuses on predicting **heart disease likelihood** using healthcare and lifestyle data.  
A **Logistic Regression** model was developed to classify patients as at-risk or not, based on parameters such as age, chest pain type, and maximum heart rate.  
Additional lifestyle features — *smoking*, *alcohol consumption*, and *exercise habits* — were integrated to improve model accuracy and real-world relevance.

---

## 🧩 Key Objectives  
- Analyze healthcare data related to heart disease  
- Apply data preprocessing, cleaning, and feature selection  
- Build a **Logistic Regression model** for prediction  
- Enhance the model using **feature engineering**  
- Evaluate performance using multiple metrics  

---

## 🧠 Dataset Details  
- **Primary Dataset:** `heart.csv` — contains medical parameters (age, cp, thalach, etc.)  
- **Lifestyle Dataset:** `lifestyle_data.csv` — includes lifestyle indicators (smoking, alcohol, exercise)  
- Both datasets were merged using a unique `patient_id` column.

---

## ⚙️ Technologies Used  
- **Programming Language:** Python  
- **Libraries:**  
  - `pandas`, `numpy` – data manipulation  
  - `matplotlib`, `seaborn` – visualization  
  - `scikit-learn` – machine learning model & evaluation  
  - `joblib` – model persistence  

---

## 🧪 Implementation Steps  

1. **Data Loading & Cleaning**
   ```python
   df = pd.read_csv('heart.csv')
   df = df.fillna(df.median(numeric_only=True))
