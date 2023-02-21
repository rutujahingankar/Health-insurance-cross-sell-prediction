# Health-insurance-cross-sell-prediction

This is a note book of  cross selling of health insurance customers on vehicle insurance product and using machine learning to predict whether a customer is interested or not in vehicle insurancen

# Background Information :
an Insurance company that provide Health Insurance to its customers, usually they offer other insurance product to the customers through diffirent kind of marketing channel. In this case we will build a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.
# Problem Statement:
Un optimize customer reachout process, many insurance worker spend a lot of their time having meeting with prospective client without knowing the probabily of that customer to buy the insurance product
# Business Goals:
Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue
# Business Question:
How does age of a vehicle determing the response of vehicle insurance advertisment
How to attract customers from different generation
what's the major factor that make a health insurance customer not intersted with vehicle insurance
What's the best machine Learning modeling for this Cross Sell case
# Exploratory Data Analysis to Answer business Question

# Feature Engineering & Selection For Machine Learning Process

# Encoding all the categorical features
Checking correlation between dependent and independet variable
Feature Selection
# Model Building :

Splitting data into Training and Testing
Apllying the SMOTE (Synthetic Minority Oversampling Technique) to the minority target since the data is imbalance
Creating base model of classification algorithm ( Logistic Regression, KNN Classifier, Decision Tree Classifier, Random Forest Clasifier)
Check The Evaluation matrix for all the base model
HyperParameter tuning
Checking Evaluation Matrix for tuned Model
Choose which model has the best recall score for this case
