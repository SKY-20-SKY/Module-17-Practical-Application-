**Bank Marketing Campaign
***Overview
The goal of this project is to compare the performance of machine learning classifiers—K-Nearest Neighbors (KNN), Logistic Regression, Decision Trees, and Support Vector Machines (SVM)—to predict if a client will subscribe to a bank term deposit.
The analysis is based on a dataset from a Portuguese banking institution involving 17 marketing campaigns conducted between May 2008 and November 2010.

Business Objective
The primary business objective is to develop a predictive model that identifies potential customers most likely to subscribe to a bank term deposit. 
By accurately targeting these individuals, the bank can improve the efficiency of its marketing campaigns and increase subscription rates.

Dataset Information
Total Records: 41,188 entries.
Features: 21 variables, including client data (age, job, marital status), contact information (month, day of week, duration), and social/economic indicators (employment variation rate, consumer price index).

Target Variable (y): "yes" if the client subscribed to a term deposit, "no" if they did not.

Exploratory Data Analysis (EDA)

Class Imbalance: The dataset is heavily skewed towards "no" responses, making it difficult for models to identify the minority "yes" class (subscribers).
Indicators such as the employment variation rate (emp.var.rate) and the 3-month Euribor rate (euribor3m) show strong positive correlations with each other but are negatively correlated with subscription rates.
Initial exploration suggests that older customers have a higher probability of subscribing.
Excessive contacts during a single campaign do not necessarily lead to better outcomes.

Models Evaluated
Tuned Logistic Regression model achieved highest precision score of 0.669 and a good test accuracy score of 0.901 making it ideal model for customers to subscribe
Tuned Decision Tree also is a close contender with a test accuracy of 0.904 and Precision of 0.612 with a very low training time.
Considering all parameters, Tuned Logistic Regression has slight edge over the tuned decision tree model

Summary of Results
While the models achieved high overall accuracy, the F1 score for the minority class remained very low across initial tests. Further data analysis is needed to adress the class imbalance
