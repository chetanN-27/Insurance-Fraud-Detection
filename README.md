# InsureNow Claims Prediction
This repository contains a machine learning solution for predicting insurance claim outcomes based on the provided dataset from InsureNow. The primary objective is to predict whether a claim will be approved, settled, or denied, while also analyzing data characteristics to assist in negotiating better terms with clients.

## Data Description
The dataset contains 12 columns across 3 datasets:

Claim Number
Incident Date - Date of Incident
Date Received - Date on which claim request was received
City Code
City
Enterprise Type - Type of the company
Claim Type
Claim Site
Product Insured - Which product is being claimed for payment
Claim Amount - Amount in Hundreds - Amount Claimed by Client
Close Amount - Amount In Hundreds - Amount Approved after Inspection and Verification
Disposition - Target Variable - States if the Claim has been Approved, Settled or Denied
Evaluation Metric
The primary evaluation metric for the models is Recall.

## Preprocessing and EDA
Before building the models, several preprocessing and exploratory data analysis (EDA) steps were performed to understand the data and its characteristics better. These include checking data sanity across all columns, calculating the average percentage of claims received when the claim is 'Settled,' and determining which product has the highest delay in reporting.

## Visualization
Visualizations were created to answer the following questions:

Do people report products with more value earlier compared to products with less value?
Does delay in reporting affect the percentage of claim received?
How does claim type and filed claim amount affect the settlement of claim amount?
Which city has reported the highest number of incidents?
Which type of claims have the highest number of incidents?

## Modelling
A baseline classification model was chosen and implemented.
Multiple classifier models, including Logistic Regression, Support Vector Classifier, Random Forest, Decision Tree, and others, were applied to improve the performance over the baseline model.

## Model Evaluation
For the implemented models, the best parameters were found using Grid search. The model performance was presented based on the given evaluation metric, Recall. The Gradient Boosting Classifier was chosen as the best-performing model among all the classifiers tested.
