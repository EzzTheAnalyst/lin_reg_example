# **Linear Regression Analysis on E-commerce Customer Data**

## This Jupyter notebook performs exploratory data analysis (EDA) and builds a linear regression model to predict yearly spending amounts based on customer behavior metrics from an e-commerce dataset.
# Overview
The project uses a dataset of 500 e-commerce customers, analyzing features like average session length, time spent on the app/website, and membership length to predict the "Yearly Amount Spent". We train a simple linear regression model and evaluate its performance using metrics like R² score, MSE, RMSE, and MAE.

# Key findings:

The model achieves a high R² score of ~0.98 on the test set, indicating strong predictive power.
"Length of Membership" is the most influential feature (highest coefficient).

# Dataset

Source: "ecommerce_csts.csv" (included in the repository).
## Columns:

### Categorical/Non-numeric: Email, Address, Avatar (dropped for modeling).
### Numeric Features: Avg. Session Length, Time on App, Time on Website, Length of Membership.
### ***Target***: Yearly Amount Spent.


### Size: 500 rows, no missing values.

# Requirements
To run this notebook, ensure you have the following Python libraries installed (Python 3.9+ recommended):
```install pandas numpy scikit-learn seaborn matplotlib```


Ensure "Ecommerce Customers.csv" is in the same directory as the notebook

## Run all cells sequentially. The notebook includes:

### Data loading and EDA (info, describe, visualizations).
### Preprocessing (feature selection, train-test split).
### Model training and evaluation.



# Model Performance

> **Test R² Score: 0.9804**
> **Train R² Score: 0.9817**
> **Test RMSE: ~10.56 (low error relative to mean target ~499)**
Coefficients (top features): Length of Membership (~62.22), Time on App (~38.55), Avg. Session Length (~25.81)

# For visualizations
(e.g., pairplots, regression plots), refer to the notebook outputs.

# Future Improvements

Try polynomial features or Ridge/Lasso regularization.
Incorporate SGDRegressor (imported but not used).
Add cross-validation for robustness.

License
This project is open-source under the MIT License. Feel free to use and modify!
