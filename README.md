# ❤️ Cardiovascular Disease Prediction  
A complete Machine Learning project for predicting the likelihood of cardiovascular disease using medical, demographic, and lifestyle data.  
This project includes full **data preprocessing**, **EDA**, **model training**, **ROC curves**, and **performance evaluation**.

---

## 📊 Project Overview
Cardiovascular diseases are one of the leading causes of death globally.  
Using patient data such as age, blood pressure, cholesterol levels, BMI, and lifestyle factors, this project builds ML models to predict whether a patient has a high risk of cardiovascular disease.
This project was further enhanced by handling class imbalance, performing hyperparameter optimization, and introducing advanced ensemble models. Model selection was based on ROC-AUC rather than accuracy to ensure better medical relevance.


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

## 🔧 Model Optimization
To improve model performance and address class imbalance:

- Applied `class_weight='balanced'` to Logistic Regression and Random Forest
- Performed hyperparameter tuning using:
  - GridSearchCV (Logistic Regression)
  - RandomizedSearchCV / GridSearchCV (Random Forest)
- Used **ROC-AUC** as the primary evaluation metric
- Reduced false negatives, which is critical in medical prediction tasks

----

## 🤖 Machine Learning Models
Models built, optimized, and evaluated:
- Logistic Regression  
- K-Nearest Neighbor  
- Calibrated Linear SVM  
- Decision Tree  
- Random Forest
- Gradient Boosting Classifier (Final Model)


**Evaluation Metrics:**
- Accuracy  
- Classification Report  
- Confusion Matrix  
- ROC Curve  
- AUC Score  

---

## 🏆 Model Performance (ROC-AUC Scores)

| Model | ROC-AUC |
|-----|--------|
| Gradient Boosting (Final Model) | ~0.79–0.80 |
| Logistic Regression (Optimized) | ~0.78 |
| Random Forest (Optimized) | ~0.77 |
| Support Vector Machine | ~0.70 |
| K-Nearest Neighbor | ~0.68 |
| Decision Tree | ~0.63 |

Gradient Boosting achieved the best performance after optimization and was selected as the final model.


---

## 📊 ROC Curve Comparison

Each model's ROC curve is plotted in the notebook to visually compare performance.

Example result:

- Logistic Regression → highest curve  
- Random Forest → nearly equal  
- SVM → moderate  
- KNN & Decision Tree → lower  

---

## 🔍 Model Explainability (SHAP)
To improve transparency and trust in predictions, SHAP (SHapley Additive exPlanations) was used to explain the final Gradient Boosting model.

SHAP analysis revealed that the most influential features were:
- Age
- Systolic blood pressure (ap_hi)
- BMI
- Cholesterol level

This helps understand how individual features contribute to cardiovascular disease predictions.

---

## 📝 Conclusion

This project demonstrates a complete end-to-end machine learning pipeline for cardiovascular disease prediction. By addressing class imbalance, optimizing models using hyperparameter tuning, and introducing Gradient Boosting, the model performance was significantly improved. SHAP explainability further enhanced interpretability, making the solution suitable for real-world healthcare decision support systems.


---

## 📬 Contact

If you have any questions or want to collaborate, feel free to reach out:

📧 Email: **[chinthala.shivani0@gmail.com)**

I'm happy to help!
