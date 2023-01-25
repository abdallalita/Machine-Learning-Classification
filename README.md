## [Bankruptcy Prediction](#Introduction-1)
## [Banknotes Authentication](#Introduction-2)
### Introduction 1
**Bankruptcy data from the Taiwan Economic Journal for the years 1999–2009**
The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined based on the business regulations of the Taiwan Stock
Exchange.
This notebook aims to build a Machine Learning model for predicting bankruptcy using **XGBoost Algorithm**.
While **Gradient Boosting** refers to a class of ensemble machine learning algorithm that can be used for both classification and regression predictive modelling
problems, **XGBoost** of **eXtreme Gradient Boosting** is an optimized an efficient implementation of the Gradient Boosting algorithm.
More about XGBoost and Gradient Boosting algorithms can be found here: [Website](https://www.nvidia.com/en-us/glossary/data-science/xgboost/)
#### Overview
The data had 6819 rows and 19 columns, with no missing values.All the independent features are continuous while the target variable is made up of labels
**{0: Not Bankrupt, 1: Bankrupt}**.
The target variable had imbalanced data which was addressed through resampling techniques and the best model was chosen compared to the baseline accuracy.
I performed hyperparameter tuning using the GridSearchCV or GridSearch Cross-validation technique, the final model was fitted using the optimal combination of 
hyperparameters.
Finally Feature importances were extracted from the model, to show the significance or predicting power of each of the features in the model for future
Feature Selection Process.

---
### Introduction 2
This dataset is about checking out the genuine and forged banknotes. In this dataset, data were taken from the images of genuine and forged banknote.
Moreover, the images are 400 by 400 pixels. To extract the features from these images, a Wavelet transform tool was used.
There are five attributes, i.e., the variance of Wavelet Transformed image, skewness of Wavelet Transformed image, curtosis of Wavelet Transformed image, the entropy of image, and class.
The notebook aims to determine the best or appropriate algorithm for predicting whether a banknote is **fake:class(1) or real:class(0)** from the features.
More about Support Vector Machine Algorithm can be found here: [SVM](https://www.analyticsvidhya.com/blog/2017/09/understaing-support-vector-machine-example-code/)
More about Naive Bayes Algorithm can be found here: [Naive Bayes](https://www.analyticsvidhya.com/blog/2015/09/naive-bayes-explained/?utm_source=blog&utm_medium=understandingsupportvectormachinearticle)

#### Overview
The data had 1374 rows and 5 column features. I performed data cleaning by renaming columns, dropping the first two rows that had irrelevant information and finally changing the data types of the features appropriately.
I then performed Exploratory Data Analysis (EDA) to get more insights about the data in terms of data distribution etc.
A comparison between **Support Vector Machine** (SVM) and **Naive Bayes** algorithm was performed based on their F1 Scores and Recall, and the model with both higher scores was considered the most appropriate, which in this case, SVM.
This maybe due to the fact that one of the main assumption of Naive Bayes algorithm, is based on the [Bayes Theorem](https://www.investopedia.com/terms/b/bayes-theorem.asp) of conditional probability and assumes that the features are independent of each other. However in our case **multicollinearity** was seen, making the algorithm not feasible.
























