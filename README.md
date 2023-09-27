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

The dataset includes credit card transactions made by European cardholders over two days in September 2013. With 492 fraudulent transactions out of 284,807, the dataset is highly unbalanced, with frauds accounting for 0.172% of the total transactions. The dataset has been transformed with PCA to maintain confidentiality. Apart from `time` and `amount`, all other features (V1, V2, ..., V28) are principal components obtained using PCA. The `time` feature represents seconds elapsed between transactions, `amount` is the transaction amount, and `class` is the label, with 1 indicating fraud and 0 otherwise.

## Project Pipeline
The project pipeline is summarized in the following steps:
1. **Data Understanding:** Load the data and understand the available features to select the most relevant for the final model.
2. **Exploratory Data Analytics (EDA):** Perform univariate and bivariate analyses, followed by feature transformations if necessary. Check for skewness in the data and address it, as it might cause issues during model building.
3. **Train/Test Split:** Utilize the k-fold cross-validation method for validation. An appropriate k value should be chosen to ensure the minority class is correctly represented in the test folds.
4. **Model Building / Hyperparameter Tuning:** Experiment with different models and fine-tune their hyperparameters to achieve the desired performance on the dataset. Explore various sampling techniques to check for better model performance.
5. **Model Evaluation:** Evaluate the models using appropriate metrics, focusing on accurately identifying fraudulent transactions due to the data imbalance.
