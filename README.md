## Bankruptcy data from the Taiwan Economic Journal for the years 1999–2009
The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined based on the business regulations of the Taiwan Stock
Exchange.
This notebook aims to build a Machine Learning model for predicting bankruptcy using **XGBoost Algorithm**.
While **Gradient Boosting** refers to a class of ensemble machine learning algorithm that can be used for both classification and regression predictive modelling
problems, **XGBoost** of **eXtreme Gradient Boosting** is an optimized an efficient implementation of the Gradient Boosting algorithm.
More about XGBoost and Gradient Boosting algorithms can be found here: (Website)[https://www.nvidia.com/en-us/glossary/data-science/xgboost/]

### Overview
The data had 6819 rows and 19 columns, with no missing values.All the independent features are continuous while the target variable is made up of labels
**{0: Not Bankrupt, 1: Bankrupt}**.
The target variable had imbalanced data which was addressed through resampling techniques and the best model was chosen compared to the baseline accuracy.
I performed hyperparameter tuning using the GridSearchCV or GridSearch Cross-validation technique, the final model was fitted using the optimal combination of 
hyperparameters.
Finally Feature importances were extracted from the model, to show the significance or predicting power of each of the features in the model for future
Feature Selection Process.

























