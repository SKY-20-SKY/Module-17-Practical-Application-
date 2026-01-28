# Bank Marketing Campaign

## Overview
* **Goal**: To compare the performance of machine learning classifiers—**K-Nearest Neighbors (KNN)**, **Logistic Regression**, **Decision Trees**, and **Support Vector Machines (SVM)**—to predict if a client will subscribe to a bank term deposit.
* **Dataset Context**: The analysis is based on a dataset from a Portuguese banking institution involving **17 marketing campaigns** conducted between May 2008 and November 2010.

## Business Objective
* **Primary Goal**: To develop a predictive model that identifies potential customers most likely to subscribe to a bank term deposit.
* **Efficiency**: By accurately targeting these individuals, the bank can improve the efficiency of its marketing campaigns and increase subscription rates.

## Dataset Information
* **Total Records**: 41,188.
* **Features**: 21 variables (Age, job, marital status, education, contact information, consumer price index etc)
* **Target Variable (y)**: 'yes/1' if the client subscribed to a term deposit, 'no/0' if they did not.

## Exploratory Data Analysis (EDA)
* The dataset is heavily skewed towards "no" responses, making it difficult for models to identify the minority "yes" class (subscribers).
* Indicators such as the **employment variation rate (emp.var.rate)** and the **3-month Euribor rate (euribor3m)** show strong positive correlations with each other but are negatively correlated with subscription rates.
* Initial exploration suggests that older customers have a higher probability of subscribing.
* Excessive contacts during a single campaign do not necessarily lead to better outcomes.

## Models Evaluated
* **Logistic Regression**: The tuned model achieved the highest **Precision score of 0.669** and a **Test Accuracy of 0.901**, making it the ideal model for identifying potential subscribers.
* **Decision Tree**: A close contender with a **Test Accuracy of 0.904** and **Precision of 0.612**, benefiting from a very low training time.
* **Comparison**: Considering all parameters, **Tuned Logistic Regression** has a slight edge over the tuned decision tree model.

## Summary of Results
* **Performance**: While the models achieved high overall accuracy, the **F1 score** for the minority class remained very low across initial tests. 
* **Next Steps**: Further data analysis is needed to address the class imbalances.
