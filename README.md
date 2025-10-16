# Salifort Motors Employee Churn Prediction

## Project Overview
Predicts employee churn for Salifort Motors using Python data science tools. 
The project includes data cleaning, EDA, and machine learning models to identify factors associated with employees leaving the company.

## Dataset
- **File:** `HR_capstone_dataset.csv`
- **Rows:** 14,999 (with duplicates removed for analysis)
- **Key Features:** Satisfaction level, last evaluation, project count, monthly hours, tenure, work accident, promotion in last 5 years, department, salary
- **Target:** `left` (1 = left, 0 = stayed)

## Workflow

1. **Data Preparation**
    - Import, inspect, and standardize feature names
    - Remove duplicates
    - Check for and discuss outliers

2. **Exploratory Data Analysis**
    - Distributions: tenure, salary band, satisfaction, department, and more
    - Visualizations: histograms and boxplots to reveal key relationships

3. **Feature Engineering**
    - Encode categorical features (`salary`, `department`)
    - One-hot encoding for department

4. **Modeling**
    - **Logistic Regression**: Baseline model, outputs classification report and confusion matrix
    - **Decision Tree**: Hyperparameter tuning with GridSearchCV
    - **Random Forest**: Grid search for best hyperparameters, evaluation with multiple metrics

5. **Evaluation**
    - Accuracy, precision, recall, F1, and ROC-AUC for each model
    - Best model: Random Forest (accuracy ~98%, ROC-AUC ~0.98 on CV)
    - Insights: Most churned employees had low satisfaction, low salary, or few/no promotions

## Results

- **Data:** Cleaned, duplicates removed, outliers checked
- **Best model:** Random Forest (CV accuracy >98%)
- **Key factors:** Low satisfaction, low salary, tenure, few promotions


