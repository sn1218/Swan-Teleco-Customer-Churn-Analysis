# Customer Churn Analysis
## Overview

This project aims to help the Customer Retention Marketing team of a telecommunications company better understand customer churn. Using customer data, the goal is to identify the demographic characteristics of customers who churn, the products they use, and the factors influencing their decision to leave. The project also focuses on predicting which customers are most likely to churn next, offering insights that can help the company design effective retention strategies.

## Objecives

The project addresses the following key questions:

* What are the demographics of customers who churn?
* What products do churners typically have?
* Why are customers churning?
* What factors most strongly influence customer churn?
* What sign-up incentives should be prioritized to reduce churn?
* Which 500 customers are most likely to churn next?
* What is the churn risk score for all customers?

The project brief and raw data are located in the 'Data and Brief' folder.

## The Project

The tools used in this project include: Python and Python libraries (pandas, numpy, matplotlib, seaborn, sklearn, statsmodels).

### Data Cleaning and Exploratory Data Analysis (EDA)

The dataset was first cleaned and explored to gain insights into churn patterns and demographic characteristics. This process is documented in the 'EDA Swan Consulting.ipynb' notebook.

Key insights were compiled into the 'Info Deck.pdf' located in the 'For Submissions' folder. This deck provides an overview of churn demographics, product usage patterns, and recommendations for which sign-up incentives could reduce churn.

### Predictive Modelling

Two approaches were explored to predict customer churn: logistic regression and classification decision trees. The experiments for these models can be found in the 'Experimenting with Predictive Models' folder.

After evaluating both methods, logistic regression was selected as the final model due to its superior performance in terms of recall, which was our priority metric. Maximising recall helps minimise false negatives, ensuring that we catch as many potential churners as possible.

The final logistic regression model and accompanying scripts are available in the 'For Submission' folder.




