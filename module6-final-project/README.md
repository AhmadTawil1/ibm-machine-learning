# 📘 Module 6 – Practice & Final Project (IBM Machine Learning)

## Overview
In this final module, I applied the **full machine learning workflow** to real-world datasets.  
The module consisted of:
1. **Practice Project** – Titanic dataset (binary classification).  
2. **Final Project** – Rainfall prediction dataset (binary classification).  
3. **Final Exam** – Summative assessment covering all six modules.

---

## 🎯 Learning Objectives
- Apply **end-to-end ML techniques** on real-world data.  
- Practice **pipeline construction and optimization**.  
- Compare multiple models using **cross-validation and hyperparameter tuning**.  
- Evaluate models with metrics suitable for **imbalanced datasets**.  
- Demonstrate **feature engineering, preprocessing, and model interpretability**.  

---

## 🛠 Practice Project: Titanic Dataset
- **Goal:** Predict passenger survival.  
- **Workflow:**  
  - Preprocessing with `ColumnTransformer` → `SimpleImputer`, `StandardScaler`, `OneHotEncoder`.  
  - Built full **Pipeline** with `RandomForestClassifier` and `LogisticRegression`.  
  - Used `StratifiedKFold` CV + `GridSearchCV` for hyperparameter tuning.  
  - Evaluated with **classification report**, confusion matrix, ROC-AUC.  
  - Mapped feature importances back to original features after One-Hot Encoding.  
- **Results:**  
  - Best weighted F1 ≈ **0.82**.  
  - Random Forest slightly outperformed Logistic Regression.  
  - Model reproducibility ensured with `random_state`.  

---

## 🌧 Final Project: Rainfall Prediction
- **Goal:** Predict whether it will rain today, based on historical weather data.  
- **Steps:**  
  - Addressed **data leakage** (removed future-dependent features).  
  - Restricted to **Melbourne metro locations** for regional consistency.  
  - Feature engineering: created **Season** from date, shifted `RainTomorrow → RainToday`.  
  - Preprocessing: pipelines for numerical (median imputation + scaling) and categorical (imputation + one-hot).  
  - Models: Random Forest, Logistic Regression.  
  - GridSearchCV with **time-aware CV**; evaluated with Accuracy, Precision, Recall, F1.  
- **Results:**  
  - Accuracy ≈ **0.84**, but recall for rainy days only ≈ **0.50**.  
  - Random Forest achieved higher overall accuracy; Logistic Regression slightly better TPR.  
  - Feature importance: **Sunshine** and **Humidity3pm** were most predictive.  

---

## 📊 Key Skills Practiced
- Handling **imbalanced datasets** (`class_weight="balanced"`).  
- Building **reusable ML pipelines** for preprocessing + modeling.  
- **Hyperparameter tuning** with GridSearchCV.  
- Comparing models fairly on the same test set.  
- **Interpretability**: Feature importances & coefficients.  
- **Model validation**: Preventing overfitting and avoiding data leakage.  

---

## ✅ Takeaways
- Accuracy alone is misleading on imbalanced data → use Precision, Recall, F1, ROC/PR curves.  
- Pipelines + ColumnTransformers = scalable, reproducible ML workflow.  
- Feature engineering (like lags, seasonality) has big impact on performance.  
- Random Forest is a strong baseline, but threshold tuning and class weights are crucial for minority class detection.  

---

## 📂 Deliverables
- **Practice Project Notebook:** Titanic survival prediction.  
- **Final Project Notebook:** Rainfall prediction classifier.  
- **Final Exam:** Completed graded assessment.  

---

## 🚀 Next Steps
- Apply the same pipeline approach to **new datasets**.  
- Explore more advanced models (XGBoost, LightGBM).  
- Focus on **model calibration & threshold tuning** for imbalanced problems.  
- Use **SHAP** for deeper feature explainability in tree models.
