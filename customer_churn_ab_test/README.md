# Customer Churn & A/B Test Analysis

## Project Overview

This project analyzes customer churn and evaluates a simulated retention email campaign using an A/B test.

The main objectives are to:

* Identify customer characteristics associated with churn.
* Perform statistical hypothesis tests.
* Design and simulate a randomized A/B test.
* Evaluate whether a retention email can reduce 30-day customer churn.
* Translate the results into a practical business recommendation.

## Business Question

Which customer characteristics are associated with churn, and does a retention email reduce 30-day customer churn?

## Dataset

The project uses the IBM Telco Customer Churn dataset, which contains information about customers, their services, contract details, charges, tenure, and churn status.

The dataset includes the target variable `Churn`.

## Tools and Libraries

* Python
* Jupyter Notebook
* pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Statsmodels

## Project Structure

```text
customer-churn-ab-test/
├── README.md
├── requirements.txt
├── notebooks/
│   └── customer_churn_ab_test.ipynb
└── data/
    └── WA_Fn-UseC_-Telco-Customer-Churn.csv
```

## Analysis

The analysis includes:

1. Data loading and quality checks
2. Data cleaning
3. Exploratory data analysis
4. Feature engineering
5. Hypothesis testing
6. A/B test design
7. Sample-size and power calculation
8. A/B test simulation
9. Statistical analysis
10. Statistical and practical significance
11. Business recommendation

## Key Findings

Several customer characteristics were associated with churn.

Customers with shorter tenure had higher churn rates. Churn was also higher among customers with higher monthly charges.

Contract type showed a strong association with churn. Month-to-month customers had substantially higher churn than customers with one-year or two-year contracts.

Other observed differences included higher churn among customers using electronic check payment, fiber optic internet service, senior citizens, and customers without online security.

The hypothesis tests provided statistical evidence of an association between contract type and churn and differences in tenure and monthly charges between churned and non-churned customers. These findings describe relationships in the data and do not establish causation.

## A/B Test Results

A simulated randomized A/B test was used to evaluate a retention email.

* Control group churn: 11.79%
* Treatment group churn: 10.96%
* Absolute difference: -0.83 percentage points
* Relative churn reduction: 7.02%
* p-value: 0.0533
* 95% confidence interval: approximately -1.67 to 0.01 percentage points

The treatment group had a lower observed churn rate, but the result was not statistically significant at the 5% level. Therefore, the experiment does not provide sufficient statistical evidence to conclude that the retention email changes 30-day churn.

## Business Recommendation

Based on this simulated experiment alone, a full rollout of the retention email is not recommended.

A further controlled experiment or additional real-world data should be collected before making a rollout decision. The expected value of reducing churn should also be compared with the cost of sending the emails and other operational costs.

## Assumptions and Limitations

The A/B test uses simulated data rather than results from a real retention campaign.

The simulation uses assumed baseline and treatment churn rates. Different real-world rates could produce different results.

The churn analysis identifies associations but does not establish causation.

The analysis focuses primarily on 30-day churn and does not evaluate all possible business outcomes, such as long-term retention, revenue, or customer lifetime value.

## Conclusion

This project combines customer churn analysis with a simulated A/B test to connect statistical analysis with a business decision.

The analysis identified several customer characteristics associated with churn. The simulated retention email showed a lower observed churn rate, but the evidence was not statistically significant at the 5% level.

Therefore, additional real-world experimentation would be appropriate before making a full rollout decision.
