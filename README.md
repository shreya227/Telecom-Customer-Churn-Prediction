# IBM Telco Customer Churn Prediction

The objective of this notebook is to present an extensive analysis of the **Customer Churn Dataset** and to predict the customer churn rate.

### Dataset Source 

* [Kaggle Dataset URL](https://www.kaggle.com/blastchar/telco-customer-churn)
* [GitHub Dataset URL](https://raw.githubusercontent.com/shreya227/Telecom-Customer-Churn-Prediction/main/Telco-Customer-Churn-Original%20Dataset.csv)


### This project also serves as assignments for the courses below - 
1. [IBM Exploratory Data Analysis for Machine Learning](https://www.coursera.org/learn/ibm-exploratory-data-analysis-for-machine-learning?specialization=ibm-machine-learning)
2. [IBM Supervised Machine Learning: Classification](https://www.coursera.org/learn/supervised-machine-learning-classification?specialization=ibm-machine-learning)

## Summary

* Dataset mostly has categorical variables
* Data is not normally distributed, performed Nonparametric Statistical tests
* Performed statistical hypothesis test to check correlation , multicollinearity
* Imbalanced dataset, did experiment with different sampling techniques(e.g stratifying, imblearn - SMOTE etc)
* Tuned Hyperparameters using Optuna
* Performed single level Stacking Ensemble with Triple Gradient boosting algorithms and classic algorithms
* Number of months the customer has stayed with the company (tenure) and the contract term of the customer (contract) are the most important features that have strong correlation with churn of the customer
* Results from statiscial hypotheses testing reflects similarity with model feature importance
* With 80/20 train/test split triple boosting stacking ensemble model achieved an AUC of ~0.85

### Built With

```
optuna==2.10.0
xgboost==0.90
catboost==1.0.1
lightgbm==2.2.3
plotly==4.4.1
scipy==1.7.1
scikit-learn==0.22.2.post1
```
