# Health-insurance-cross-sell-prediction

This is a note book of  cross selling of health insurance customers on vehicle insurance product and using machine learning to predict whether a customer is interested or not in vehicle insurancen

## Background Information :
an Insurance company that provide Health Insurance to its customers, usually they offer other insurance product to the customers through diffirent kind of marketing channel. In this case we will build a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.
## Problem Statement:
Un optimize customer reachout process, many insurance worker spend a lot of their time having meeting with prospective client without knowing the probablity of that customer to buy the insurance product
## Business Goals:
Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue
## Business Question:
How does age of a vehicle determing the response of vehicle insurance advertisment
How to attract customers from different generation
what's the major factor that make a health insurance customer not intersted with vehicle insurance
What's the best machine Learning modeling for this Cross Sell case


## Feature Engineering & Selection For Machine Learning Process

Encoding all the categorical features
Checking correlation between dependent and independent variable
Feature Selection
## Model Building :

Splitting data into Training and Testing
Apllying the SMOTE (Synthetic Minority Oversampling Technique) to the minority target since the data is imbalance
Creating base model of classification algorithm ( Logistic Regression, Random Forest Clasifier)
Check The Evaluation matrix for all the base model
HyperParameter tuning
Checking Evaluation Matrix for tuned Model
Choose which model has the best recall score for this case

## Conclusion:
 Starting from loading our dataset, we initially checked for null values and duplicates. There were no null values and duplicates so treatment of such was not required.
Through Exploratory Data Analysis,we observed that customers belonging to youngAge are more interested in vehicle response.while Young people below 30 are not interested in vehicle insurance. We observed that customers having vehicles older than 2 years are more likely to be interested in vehicle insurance. Similarly, customers having damaged vehicles are more likely to be interested in vehicle insurance.
The variable such as Age, Previously_insured,Annual_premium are more afecting the target variable.
For Feature Selection, we applied the Mutual Information technique. Here we observed that Previously_Insured is the most important feature and has the highest impact on the dependent feature and there is no correlation between the two.
We observed that the target variable was highly imbalanced.So this issue was solved by using Random Over Sample resampling technique.
we applied feature scaling techniques to normalize our data to bring all features on the same scale and make it easier to process by ML algorithms.
Further, we applied Machine Learning Algorithms to determine whether a customer would be interested in Vehicle Insurance.For the logistic regression we got an accuracy of 78% and for the XGBClassifier we got the aacuracy of 79% whereas, Randomforest and Decision tree are giving us almost similar result of accuracy and ROC_AUC which is 91% and 92% respectively.So, we selected our best model as the model with an accuracy score of 91% i.e Random Forest model and Decision Tree this model preform better.
