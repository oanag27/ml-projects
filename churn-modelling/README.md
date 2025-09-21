# 🏦 Customer Churn Prediction

This project predicts **customer churn** (whether a bank customer will leave or stay) using machine learning.  
The dataset comes from Kaggle: [Churn Modelling Dataset](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling/data).

## 📊 Dataset
- **Rows:** 10,000 customers  
- **Features:** Credit score, geography, gender, age, tenure, balance, number of products, etc.  
- **Target:** `Exited` (1 = customer left, 0 = customer stayed)

## ⚙️ Project Workflow
1. **Data Preprocessing**
   - Handled missing values
   - Converted categorical variables (`Gender`, `Geography`) into numerical
   - Scaled numerical features

2. **Model Training**
   - Tested ML algorithms (RandomForestClassifier, LogisticRegression, SVC, GradientBoostingClassifier)

3. **Evaluation**
   - Metrics used:
     - Accuracy
     - Classification Report
     - Confusion Matrix

## 📈 Results

| Model                  | Accuracy |
|-------------------------|----------|
| Random Forest           | 85.8%    |
| Logistic Regression     | 81.2%    |
| SVM (linear kernel)     | 79.9%    |
| Gradient Boosting       | 86.4%    |
