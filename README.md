![Header](header.png)

## Introduction

In recent years, the E-commerce company has experienced good customer growth, but recent data shows an increase in the number of customers who Churn from the E-Commerce website.

To retain profitability growth, the company can employ two strategies:
 1. Retain existing customers
 2. Acquire new customers
In research findings that customer acquisition costs are five times higher than customer retention costs.

## Problem Statements

One of the challenges faced by e-commerce businesses is to retain customers and ensure they continue making transactions.

## Goals

In many business scenarios, retaining customers or detecting customers who are likely to switch to competitors can be more important than attracting new customers. In this case, focusing on recall can help identify customers who might leave our platform or service, allowing for more proactive measures to retain them.

## Analytic Approach

Here are the steps of the analysis which will undertake:

Step-1: Conduct Exploratory Data Analysis (EDA).
Step-2: Build a classification model based on behavioral analysis.
Step-3: Identify the factors that contribute to the likelihood of customers Churning.
Step-4: Develop a simulated scheme/strategy.

The analysis results can be accessed by stakeholders through a dedicated platform (Web/Mobile) whenever they need to perform retention activities. 

## Metric Evaluation

Target:

0: customer does not churn

1: customer churns

Confusion Matrix Terms:

TP (True Positive): customer actually churns and is predicted to churn<br>
TN (True Negative): customer actually does not churn and is predicted not to churn<br>
FN (False Negative): customer actually churns and is predicted not to churn<br>
FP (False Positive): customer actually does not churn and is predicted to churn<br>

Cost of FN (False Negative):

Disadvantages:

* Loss of a customer (churn) costing $100 per customer<br>
* Cost of customer acquisition to replace the churned customer at $500 per customer<br>

Cost of FP (False Positive):

Advantages:

* As a result of mistakenly treating a customer who does not actually churn but is predicted to churn, the e-commerce platform's reputation may improve (non-churning customers will think the platform is generous in giving out promotions for free)

Disadvantages:

* Miss-targeted treatment for customers who do not churn (but are predicted to churn)
* Waste of customer retention costs, time, and resources

Based on these consequences, what I aim to do is create a model that can optimize the customer retention costs for the company without any customers churning from the e-commerce website. Therefore, I decide to emphasize False Negatives, but also not forget about False Positives, with a greater focus on recall. Hence, the focus metric we use is the F2-Score.

**Reference**:
- https://www.paddle.com/resources/customer-acquisition-vs-retention


## Project Organization
    .
    ├── README.md
    ├── data
    │   ├── E-commerce Customer Churn.docx
    │   ├── data_ecommerce_customer_churn.csv
    │   ├── data_seen.csv
    │   ├── data_unseen.csv
    │   └── saved_nb_model.pkl
    ├── docs
    ├── header.png
    ├── logs.log
    ├── requirements.txt
    └── src
        └── E-commerce_churn.ipynb

## Contribute

If you'd like to contribute to Supermarket_Customer_Analysis, check out https://github.com/priscillahilary/ML_Capstone3.git, or feel free to contact me.