# Credit Card Fraud Detection Project

## Problem Statement
The chosen problem statement for this project is to predict fraudulent credit card transactions utilizing machine learning models.

In this project, I will analyze customer-level data, collected and analyzed during a research collaboration between Worldline and the Machine Learning Group.

The dataset is sourced from the [Kaggle website](https://www.kaggle.com/mlg-ulb/creditcardfraud) and consists of 284,807 transactions, with 492 of them being fraudulent. Given the high imbalance in the dataset, it is imperative to address this issue before proceeding with model building.

## Business Problem Overview
For numerous banks, retaining highly profitable customers is the paramount business goal. However, banking fraud significantly threatens this objective. It results in substantial financial losses and undermines the trust and credibility of banks.

According to the Nilson Report, banking frauds were projected to account for $30 billion worldwide by 2020. The proliferation of digital payment channels has also seen an increase in the number of fraudulent transactions.

In the banking industry, leveraging machine learning for credit card fraud detection has evolved from a trend to a necessity. It enables banks to implement proactive monitoring and fraud prevention mechanisms, reducing time-consuming manual reviews, costly chargebacks, fees, and denials of legitimate transactions.

## Understanding and Defining Fraud
Credit card fraud is any dishonest act to obtain information without proper authorization from the account holder for financial gain. Among various methods, skimming is most prevalent, involving the duplication of information located on the card's magnetic strip. Other methods include:
- Manipulation/alteration of genuine cards
- Creation of counterfeit cards
- Stealing/loss of credit cards
- Fraudulent telemarketing

## Data Dictionary
The dataset can be downloaded [here](https://www.kaggle.com/mlg-ulb/creditcardfraud).

The dataset includes credit card transactions made by European cardholders over two days in September 2013. With 492 fraudulent transactions out of 284,807, the dataset is highly unbalanced, with frauds accounting for 0.172% of the total transactions. The dataset has been transformed with PCA to maintain confidentiality. Apart from `time` and `amount`, all other features (V1, V2, ..., V28
