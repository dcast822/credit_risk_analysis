# Credit Risk Analysis

## Problem Statement

How would you improve the bank's existing state-of-the-art credit scoring of borrowers? How will you predict someone can face financial distress in the next couple of years?
* Think about how we gauge financial distress from a banking perspective?  Can we predict whether a borrower will default or not?
* What features most heavily contribute to whether a client will default or not?

## Dataset

This is simulated credit bureau data taken from kaggle here : [Kaggle Simulated Credit Bureau Data](https://www.kaggle.com/datasets/laotse/credit-risk-dataset).

### Data Dictionary
| Feature Name               | Description                                                   |
|----------------------------|---------------------------------------------------------------|
| person_age                 | Age                                                           |
| person_income              | Annual income                                                 |
| person_home_ownership      | Home Ownership Status                                         |
| person_emp_length          | Length of employment (years)                                  |
| loan_intent                | Loan Intent                                                   |
| loan_grade                 | Loan Grade                                                    |
| loan_amnt                  | Loan amount                                                   |
| loan_int_rate              | Interest Rate                                                 |
| loan_status                | If person has defaulted or not (0 = non-default, 1 = default) |
| loan_percent_income        | Loan as percent of income                                     |
| cb_person_default_onfile   | If person has defaulted in the past                           |
| cb_person_cred_hist_length | Credit History Length                                         |


## Data Visualizations & Analysis

![Aggregations!](./images/aggregations.png "Aggregations")

Great way to see if there is anything out of the ordinary;
* Max  age of 144 & employment length of 123 are a few of the things that do not add up.

### Histogram Overview
![Histogram!](./images/numeric_dist_plots.png "Histogram")

* Most people in the data set are in between their 20s and 30s
* Most people stay at a job for less than 10 years.
* Most of the population has a loan amount of between 5,000 to 10,000
* Most of the people in the distribution have a loan to income percent of less than 25 %.

### Employment length

![Employment Length Histogram!](./images/emp_length_hist_og.png "Employment Length Histogram")
* Right skewed heavily due to what appears to be outliers reaching past the 120 year mark.

![Employee Length Boxplot!](./images/emp_length_original_boxplot.png "Employee Length Boxplot")

* Clear outliers occur from about the 20 year mark on, interquartile range calculations can give us a specific threshold by which to eliminate them.

![Employee Length Boxplot(Post Outliers)!](./images/box_emp_length.png "Employee Length Boxplot(Post Outliers)")
* Post dealing with outliers the cutoff is 14 years.

![Distribution of Employment Length By Loan Status!](./images/person_emp_hist_loan_status.png "Distribution of Employment Length By Loan Status")
* As we drill down by employee length and loan status, we see both frequency of both populations go down over time at the same about the same proportional rate.
### Personal Income(Annual)

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")

![!](./images/.png "")
