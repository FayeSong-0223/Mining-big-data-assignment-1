# 🧠 Obesity Prediction using Health Indicators

This project applies **machine learning classification techniques** to predict obesity levels based on a range of health and lifestyle indicators. It was developed as part of the *Mining Big Data* course, with a focus on the **complete machine learning workflow**, from data analysis and preprocessing to model evaluation and recommendation.

## 📌 Objective

To construct, train, and evaluate models that classify obesity categories using health-related features, and to interpret the influence of different factors on obesity levels. This task also aims to support health-related policy-making through data-driven recommendations.

---

## 📂 Project Structure

- `obesity_prediction_assignment.ipynb`: Complete Jupyter Notebook with code, charts, model evaluation, and discussions.
- `ObesityDataSet.csv`: Raw dataset with lifestyle, demographic, and health-related features.
- `README.md`: Project documentation (this file).

---

## 🔍 Methodology Overview

This project follows a standard supervised learning pipeline for **classification**:

### 1. **Data Exploration & Visualization**
- Preview of dataset structure and statistical summary
- Distribution plots of obesity categories and numerical features
- Correlation heatmap to understand feature relationships

### 2. **Data Preprocessing**
- **Missing value checks** and cleaning
- **BMI calculation** as an additional feature (`BMI = Weight / Height²`)
- **Label encoding** for target variable (`NObeyesdad`)
- **One-hot encoding** for categorical variables
- **Feature scaling** using Standard Scaler for numerical features

> All preprocessing steps are fully explained and reproducible.

### 3. **Model Implementation**
Two candidate classification models were trained:
- `Logistic Regression`
- `Random Forest`

Selection rationale:
- `Logistic Regression` is a strong baseline for linear relationships and interpretability.
- `Random Forest` is robust to multicollinearity and handles categorical interactions effectively.

### 4. **Model Training & Evaluation**
- **Train-test split** (stratified 70-30 split to preserve class balance)
- Performance metrics used:
  - Accuracy
  - Classification Report (Precision, Recall, F1-score)
  - Confusion Matrix
- Comparison of models based on performance
- Visual analysis of top 10 feature importances from the best-performing model

---

## 🧠 Key Findings

- `Weight`, `BMI`, and `CAEC` (frequency of calorie consumption) showed the strongest correlation with obesity levels.
- `Random Forest` outperformed `Logistic Regression` in both accuracy and robustness.
- Final selection: **Random Forest**, due to its higher classification accuracy and clearer feature importance extraction.

---

## ✅ Health Recommendations

Based on model findings:

- Frequent consumption of high-calorie food (e.g., `CAEC = Frequently`) and sedentary lifestyle are strong obesity predictors.
- Targeted public health campaigns should emphasize:
  - Reducing passive transport (MTRANS)
  - Encouraging regular exercise routines
  - Controlling frequency of high-calorie food intake

These interventions may be prioritized based on variable influence weights derived from the model.

---

## 💬 Reflection

Through this project, I developed practical proficiency in:
- Building and evaluating machine learning classifiers on structured data
- Handling real-world preprocessing challenges (encoding, scaling, feature engineering)
- Understanding model interpretability and communicating technical insights with charts
- Translating model findings into actionable recommendations

This assignment also reinforced the importance of fairness in evaluation and the ethical use of health data.

---

## 📚 References

- Pedregosa, F., Varoquaux, G., Gramfort, A., et al. (2011). *Scikit-learn: Machine Learning in Python*. Journal of Machine Learning Research, 12, 2825–2830.
- Course materials from *Mining Big Data* workshops and seminars (University of Adelaide, 2025)

---

## 👤 Author

**Ziqi Song**  
Master of Computing and Innovation  
University of Adelaide  
GitHub: [FayeSong-0223](https://github.com/FayeSong-0223)
