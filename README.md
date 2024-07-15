# Customer Churn Analysis
## The Scenario

The Customer Retention Marketing team of a telecommunications company would like to use data about customers that churn and customers that stay to inform their decision making. 

They would like to know the demographic of churners, what products the have, and why they are churning. They would like to know what factors influence someone churning, and what sign up factors they should incentivise. They would also like a list of the 500 customers most likely to churn next, and a list of the customer churn risk.

The project brief and data can be found in the 'Data and Brief' folder.

## The Project

The tools used in this project include: Python and Python libraries (pandas, numpy, matplotlib, seaborn, sklearn, statsmodels).

The data is first cleaned and exploratory data analysis is performed in the 'EDA Swan Consulting.ipynb' document. From the insights gained through the EDA, an information deck has been produced describing the demographic of churners, the products they buy, and what sign up factors to incentivise, see the 'Info Deck.pdf' within the 'For Submissions' folder.

Both logistic regression and classification decision trees were explored as a method to predict which customers will churn next. Notebooks exploring these can be found in the 'Experimenting with Predictive Models' folder. The final models are in the 'For Submission' folder.

In the end, three separate models were produced, with logistic regression performing best in terms of the metrics that we wanted to maximise (maximise recall to minimise false negatives). The two lists were produced using the weighted average of all three models.




