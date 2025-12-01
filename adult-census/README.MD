# Adult Census Income

Predict whether income exceeds $50K/year

The dataset comes from Kaggle: [Adult Census Income](https://www.kaggle.com/datasets/uciml/adult-census-income).


## ⚙️ Project Workflow
1. **Data Preprocessing**
    - Replaced missing values (?) with "Unknown"
    - Applied one-hot encoding to categorical variables (workclass, occupation, native.country, relationship, race, marital.status).
    - Encoded binary categorical features
  
2. **Model Training**
    - Random Forest Classifier
    - Hyperparameter tuning using GridSearchCV
   
3. **Evaluation**
    - Feature importance analysis

## 📈 Results

| Model                      | Accuracy |
|----------------------------|----------|
| Random Forest              | 0.8519   |
| Random Forest after tuning | 0.8618   |
