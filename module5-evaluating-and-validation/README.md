# 📘 Module 5: Model Evaluation & Validation  

This module covers how to properly evaluate and validate machine learning models to ensure they generalize well to unseen data.  
It introduces key evaluation metrics, pitfalls like data leakage, and advanced techniques such as cross-validation, regularization, and hyperparameter tuning with pipelines.  

---

## 📂 Topics Covered  
- **Classification Metrics**: Accuracy, Precision, Recall, F1, ROC, AUC  
- **Regression Metrics**: MAE, MSE, RMSE, R²  
- **Clustering Evaluation**: Silhouette Score, Inertia, Davies-Bouldin Index  
- **Train/Validation/Test Split** and **Data Snooping Risks**  
- **Cross-Validation & Stratified CV** for fair evaluation  
- **Regularization**: Ridge (L2), Lasso (L1), feature shrinkage and selection  
- **Pipelines & GridSearchCV**: safe hyperparameter tuning and preprocessing  

---

## 🧪 Labs Completed  
1. **Evaluating Classification Models**  
   - Built confusion matrix, calculated precision, recall, F1, and plotted ROC/AUC.  
   - Understood trade-offs between false positives and false negatives.  

2. **Evaluating Random Forest Models**  
   - Compared train vs test accuracy to detect overfitting.  
   - Interpreted feature importance.  

3. **Evaluating K-Means Clustering**  
   - Measured cluster quality using silhouette score, inertia, and Davies-Bouldin index.  
   - Explored how different values of K impact clustering results.  

4. **ML Pipelines & GridSearchCV**  
   - Constructed full ML pipelines (scaling → PCA → classifier).  
   - Used GridSearchCV for hyperparameter tuning with cross-validation.  
   - Prevented data leakage by applying transformations inside folds.  

5. **Regularization in Linear Regression**  
   - Compared Linear, Ridge, and Lasso regression.  
   - Observed how Ridge shrinks coefficients and Lasso performs feature selection.  
   - Evaluated using MSE and coefficient analysis.  

---

## 🔑 Key Takeaways  
- Always evaluate on **unseen data** (test set must remain untouched until the end).  
- Different tasks require different metrics (accuracy ≠ always best).  
- **Cross-validation** gives more reliable estimates than a single split.  
- **Regularization** controls overfitting by shrinking coefficients.  
- **Pipelines + GridSearchCV** = clean, leakage-free hyperparameter tuning.  

---