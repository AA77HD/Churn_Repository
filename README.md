# Churn_Repository
Customer Churn Prediction

Overview
This project was developed as part of my Data Science Bootcamp at TripleTen.
The main goal was to analyze customer behavior and build a model that predicts whether a customer will leave (churn).
I worked with real-world telecom-style data to understand what factors influence customer decisions, and used machine learning to help anticipate which customers are at risk of leaving.

Objectives
Perform an exploratory analysis to understand the churn patterns.
Build a predictive model capable of identifying customers likely to churn.
Evaluate different machine learning algorithms and compare their performance.
Translate results into insights that can help reduce customer churn.

Process Summary

Data Preparation
Cleaned missing values and formatted categorical features.
Scaled numerical variables with StandardScaler.
Balanced the dataset using SMOTE to fix class imbalance.

Exploratory Data Analysis (EDA)
Explored customer demographics and contract types.
Found strong churn correlation with month-to-month contracts and payment methods.
Visualized feature relationships using Matplotlib and Seaborn.

Model Training

Tested and compared several models:
Logistic Regression
Random Forest
XGBoost
Used metrics like ROC-AUC, Precision, Recall, and F1-score to evaluate each model.

Results
Model	ROC-AUC	Accuracy	Precision	Recall
Logistic Regression	0.85	0.79	0.76	0.74
Random Forest	0.89	0.83	0.80	0.77
XGBoost	0.91	0.85	0.82	0.81

The final model selected was XGBoost, as it achieved the best balance between accuracy and recall.

Tools and Libraries

Python
Pandas, NumPy, Matplotlib, Seaborn
Scikit-learn, XGBoost
Jupyter Notebook

Key Insights

Customers with month-to-month contracts were much more likely to churn.
Electronic check payments had the highest churn rate among payment methods.
Customers with longer contracts or bundled services tended to stay longer.
The model could help reduce churn by around 20–25% with proactive retention actions.

Files Included

churn_prediction.ipynb → main notebook with analysis, modeling, and conclusions.
data/ → datasets used for training and testing.
requirements.txt → libraries needed to reproduce the project.
