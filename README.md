# Social Network Ads Classification  

Comparative analysis of multiple machine learning models to predict whether a customer will purchase a product after clicking a social media advertisement.  

This project benchmarks **Decision Tree, Logistic Regression, Random Forest, XGBoost, KNN, and SVM** (both default and hyperparameter-tuned versions) to evaluate their classification performance.  

---

## 📊 Dataset  
- **Source:** Social Network Ads dataset (common ML practice dataset)  
- **Features:** Age, Estimated Salary  
- **Target:** Purchased (1 = Yes, 0 = No)  

---

## 🚀 Models Evaluated
- Decision Tree (Default & Tuned)  
- Logistic Regression (Default & Tuned)  
- Random Forest (Default & Tuned)  
- XGBoost (Default & Tuned)  
- KNN (Default & Tuned)  
- SVM (Default & Tuned)  

---

## ⚙️ Methodology
1. Data preprocessing & scaling  
2. Train-test split (80/20)  
3. Model training (default and tuned with GridSearchCV)  
4. Cross-validation for stability check  
5. Performance evaluation using:
   - Accuracy  
   - ROC-AUC Score  
   - Confusion Matrix  
   - Classification Report (Precision, Recall, F1-Score)  
   - Comparative visualization  

---

## 📈 Results Summary

| Model                          | Accuracy | ROC-AUC | Key Notes |
|--------------------------------|----------|---------|-----------|
| Decision Tree (Default)        | 91.7%    | 0.958   | Improved slightly with tuning |
| Logistic Regression (Default)  | 85.0%    | 0.958   | Good ROC but weaker accuracy |
| Random Forest (Default/Tuned)  | 95.0%    | 0.972   | **Top performer, stable** |
| XGBoost (Default)              | 89.2%    | 0.972   | Tuned version slightly worse |
| KNN (Default/Tuned)            | 93.3%    | **0.980** | Highest ROC-AUC |
| SVM (Default/Tuned)            | 94.2%    | 0.978   | Strong & consistent |

---

## 📊 Accuracy Comparison, Confusion Matrix and ROC-Curve Plot are stored in the results folder.
*(Barplot comparing model accuracy — Random Forest, SVM, and KNN are leading performers.)*  
And similarly, other plots have been shown up.
---

## ✅ Key Takeaways
- **Random Forest, SVM, and KNN** achieved the highest performance.  
- **Tuning improved Decision Tree and Logistic Regression** but had little effect (or a negative effect) on others.  
- **KNN gave the best ROC-AUC (0.98)**, while **Random Forest achieved the highest accuracy (95%)**.  
- Logistic Regression remains a solid baseline but lags behind ensemble and kernel-based models.  

---

## 📦 Tech Stack
- Python  
- scikit-learn  
- XGBoost  
- matplotlib, seaborn, pandas, numpy  

---

