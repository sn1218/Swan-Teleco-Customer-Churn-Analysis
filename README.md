# Customer Churn Analysis
## Overview

This project aims to assist the Customer Retention Marketing team of a telecommunications company in understanding customer churn and predicting which customers are at risk of leaving. By analysing customer data, the project identifies demographic patterns, product usage, and key factors influencing churn, providing actionable insights for retention strategies. Additionally, the project predicts the 500 customers most likely to churn next and calculates a churn risk score for all customers to help prioritize marketing efforts.

## Objecives

This project addresses several key business questions:

* **Demographics:** What are the demographic characteristics of customers who churn?
* **Product Usage:** What products and services do churners typically use?
* **Churn Reasons:** What are the primary reasons behind customer churn?
* **Key Influencers:** What factors have the strongest impact on customer churn?
* **Retention Strategies:** Which sign-up incentives should be prioritized to reduce churn?
* **High-Risk Customers:** Which 500 customers are most likely to churn next?
* **Churn Risk Score:** What is the churn risk score for all customers?

The project brief, along with raw data, can be found in the 'Data and Brief' folder.

## Project Details
### Tools and Libraries
This project was implemented in Python and utilised several key libraries, including:

* **pandas and numpy:** For data manipulation
* **matplotlib and seaborn:** For visualising the data
* **sklearn and statsmodels:** For building and evaluatiing machine learning models (logistic regression and decision trees)

### Dataset
The dataset contains information on customers, their demographics, product usage, and whether or not they churned. It provides a comprehensive view of customer interactions with the company, including:

* **Demographic Information:** Gender, partner, dependents, location, etc.
* **Service Information:** Types of products and services subscribed to.
* **Churn Label:** A binary label indicating whether the customer has churned (1) or not (0).

The dataset is stored in the 'Data and Brief' folder and was cleaned and preprocessed for analysis and modeling.

### Data Cleaning and Exploratory Data Analysis (EDA)

The data cleaning and EDA processes are fully documented in the 'EDA Swan Consulting.ipynb' notebook, which provides insights into the patterns and trends in customer churn.

Key findings from the EDA are summarised in the 'Info Deck.pdf' located in the 'For Submissions' folder. The deck provides:

* Demographic breakdowns of churners.
* Product usage patterns among customers who churned.
* Insights into why customers are leaving and recommendations for sign-up incentives that could reduce churn.

### Predictive Modelling

Two approaches were explored to predict customer churn: logistic regression and classification decision trees. 

The final prediction model was developed by taking a weighted average of the predicted probabilities from all three models, weighted by the recall of each model. Prioritising recall helps reduce false negatives, ensuring that the model captures as many potential churners as possible.

The detailed experimentation process is available in the 'Experimenting with Predictive Models' folder, where different models were trained, tested, and compared using performance metrics. The combined model can be found in 'closeness_checking.ipynb' in the 'For Submission' folder.

#### Model Performance
* **Logistic Regression (SN):** Recall: 82%, Precision: 53% (on test data).
* **Logistic Regression (TC):** Recall: 81%, Precision: 51% (on test data).
* **Random Forest:** Recall: 77%, Precision: 52% (on test data).

The final combined model improves prediction accuracy by averaging the probability predictions from all three models, weighted by their recall performance. This allows for a more balanced identification of potential churners.

## Repository Structure
* Data and Brief: Folder containing the raw data and project brief.
  * 0 - Project Info.pdf: Project brief
  * 1 - Project Data.xlsx: Project data in Excel format.
  * swan_data.csv: Project data in csv format.
* Experimenting with Predictive Models: Folder containing experiments with different predictive models, including logistic regression and random forest. Each model generates a CSV file of high-risk churners and churn probabilities.
* For Submission: Folder containing the final models, the combined model, and all necessary artifacts for submission.
  * EDA Swan Consulting.ipynb: Jupyter notebook for data cleaning and exploratory data analysis.
  * Info Deck.pdf: Slide deck summarising key findings from the EDA.
  * Logistic Regression SN.ipynb: Logistic regression model with a recall of 82%.
  * Logistic Regression TC.ipynb: Logistic regression model with a recall of 81%.
  * Random Forest Modelling.ipynb: Random forest model with a recall of 77%.
  * closeness_checking.ipynb: Notebook for calculating the weighted average of the three models’ predictions.
  * combined_churn_risk.csv: Churn risk score for all customers from the combined model.
  * combined_top_500.txt: List of the top 500 customers most likely to churn, as predicted by the combined model.

## How to Use the Project
1. Clone the repository and download the dataset and notebooks.
2. Open the 'EDA Swan Consulting.ipynb' to explore customer churn patterns and the preprocessing steps.
3. Run the logistic regression and random forest models to generate churn predictions for each model. The models will output CSV files containing the results.
4. Run the 'closeness_checking.ipynb' notebook to combine the predictions from all three models, generate final churn risk scores for all customers, and identify the top 500 high-risk customers.


