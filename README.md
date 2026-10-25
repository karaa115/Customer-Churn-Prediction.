
# Customer Churn Prediction

## About the Project

In this project, I analyzed customer data from a telecommunications company to understand why customers leave and which customers are more likely to cancel their services.

I wanted to see how contract types, monthly charges, and customer tenure are related to churn. I also trained two machine learning models to predict which customers might leave.

## Data Analysis

The dataset contains 7,032 customers. I started by checking the data, exploring customer behavior, and comparing customers who stayed with those who left.

Around 26.6% of customers had churned.

## Machine Learning

I trained and compared two models:
- Logistic Regression
- Random Forest

I split the data into 80% for training and 20% for testing.

### Model Results

| Metric | Logistic Regression | Random Forest |
|---|---|---|
| Accuracy | 79.4% | 79.2% |
| Precision | 63.5% | 63.9% |
| Recall | 52.7% | 50.5% |
| F1-score | 0.576 | 0.564 |
| ROC-AUC | 0.835 | 0.835 |

Both models performed similarly. Logistic Regression had slightly better recall and F1-score.

I also checked the confusion matrices, tested different classification thresholds, and used cross-validation to compare model performance.

## What I Found

The Random Forest model showed that some of the most important features for predicting churn were:

- Customer tenure
- Total charges
- Month-to-month contracts
- Monthly charges
- Online security services

I also grouped customers into three churn risk levels.

| Risk Level | Customers | Actual Churn Rate |
|---|---:|---:|
| Low | 846 | 10.52% |
| Medium | 352 | 40.62% |
| High | 209 | 67.94% |

Customers in the high-risk group had a much higher churn rate than those in the low-risk group.

These results could help a telecommunications company identify customers at risk of leaving and plan retention activities.

## Tools

Python, Pandas, NumPy, Matplotlib, Scikit-learn, SciPy, Jupyter Notebook.

