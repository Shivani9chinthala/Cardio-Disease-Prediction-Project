# ❤️ Cardiovascular Disease Prediction  
A complete Machine Learning project for predicting the likelihood of cardiovascular disease using medical, demographic, and lifestyle data.  
This project includes full **data preprocessing**, **EDA**, **model training**, **ROC curves**, and **performance evaluation**.

---

## 📊 Project Overview
Cardiovascular diseases are one of the leading causes of death globally.  
Using patient data such as age, blood pressure, cholesterol levels, BMI, and lifestyle factors, this project builds ML models to predict whether a patient has a high risk of cardiovascular disease.

This repository includes:
- Complete **EDA with visualizations**
- Feature engineering (Age in years, BMI)
- Model training with:
  - Logistic Regression  
  - K-Nearest Neighbor (KNN)  
  - Support Vector Machine (Calibrated Linear SVC)  
  - Decision Tree  
  - Random Forest  
- **ROC-AUC comparison of all models**
- Feature importance visualization

---


---

## 🧠 Dataset Information

**Features used:**
- `age_years`
- `gender`
- `height`
- `weight`
- `ap_hi` (systolic BP)
- `ap_lo` (diastolic BP)
- `cholesterol`
- `gluc`
- `smoke`
- `alco`
- `active`
- `bmi`

**Target Variable:**  
`cardio`  
- 0 → No disease  
- 1 → Disease present  

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 📈 Exploratory Data Analysis (EDA)
The notebook contains:
- Distribution plots (Age, BMI, BP, Height, Weight)
- Gender vs Cardio distribution
- Cholesterol & Glucose level analysis
- Correlation heatmap
- Boxplots & violin plots
- Scatterplots (BMI vs BP)
- Pairplots

Visualizations help identify patterns indicating cardiovascular risk.

---

## 🤖 Machine Learning Models
Models built and evaluated:
- Logistic Regression  
- K-Nearest Neighbor  
- Calibrated Linear SVM  
- Decision Tree  
- Random Forest  

**Evaluation Metrics:**
- Accuracy  
- Classification Report  
- Confusion Matrix  
- ROC Curve  
- AUC Score  

---

## 🏆 Model Performance (AUC Scores)

| Model | AUC Score |
|-------|----------|
| **Logistic Regression** | **0.778** |
| Random Forest | 0.771 |
| Support Vector Machine | 0.703 |
| K-Nearest Neighbor | 0.686 |
| Decision Tree | 0.630 |

Logistic Regression performs best on this dataset, closely followed by Random Forest.

---

## 📊 ROC Curve Comparison

Each model's ROC curve is plotted in the notebook to visually compare performance.

Example result:

- Logistic Regression → highest curve  
- Random Forest → nearly equal  
- SVM → moderate  
- KNN & Decision Tree → lower  

---

## 📝 Conclusion

The project demonstrates that machine learning models can effectively predict cardiovascular risk using basic health metrics. Logistic Regression and Random Forest achieve the best performance, making them suitable for early risk detection systems in healthcare applications.
