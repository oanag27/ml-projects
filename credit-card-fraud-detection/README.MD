# Credit Card Fraud Detection

This project detects **fraudulent credit card transactions** using machine learning.  
The dataset comes from Kaggle: [Credit Card Fraud Detection Dataset 2023](https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023/data).

## 📊 Dataset
- **Rows:** 142,907 transactions  
- **Features:** 28 anonymized features (`V1`–`V28`), `Amount`  
- **Target:** `Class` (0 = non-fraud, 1 = fraud)  

## ⚙️ Project Workflow
1. **Data Preprocessing**
   - Removed `id` column
   - Scaled numerical features using `StandardScaler`
   - Split data into train and test sets

2. **Model Training**
   - Random Forest Classifier
   - Hyperparameters:
     - `n_estimators=100`
     - `max_depth=10`
     - `min_samples_split=5`
     - `random_state=50`
   - Used 2-fold cross-validation

3. **Evaluation**
   - Metrics:
     - F1-score
     - Precision, Recall
     - Classification Report
   - Feature importance analysis

## 📈 Results

| Metric / Classifier       | Score         |
|---------------------------|---------------|
| Cross-validation F1-score | 0.984         |
| Test Accuracy             | 0.99          |
| Precision (fraud)         | 1.00          |
| Recall (fraud)            | 0.97          |
| Top Feature               | V14 (0.166)   |
| Other Important Features  | V4, V10, V12, V17 |

## 🔍 Visualizations
- **Feature Importance Bar Chart**: Highlights top contributors to fraud detection  
- **Correlation Matrix Heatmap**: Shows relationships between features  