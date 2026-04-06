# Telco Customer Churn Prediction

This project is an end to end machine learning system designed to predict customer attrition for a telecommunications company. By analyzing customer behavior and demographics, the system identifies individuals at risk of leaving, allowing for proactive retention strategies.

The project covers the entire data science lifecycle, from initial data cleaning to model evaluation and final deployment.


## Tech Stack

 **Language:** Python (3.10+ recommended)
 **Core Libraries:** `pandas`, `numpy`, `scikit-learn`, `imbalanced-learn`, `xgboost`, `matplotlib`, `seaborn`, `scipy`
 **Environment Management:** `uv` + virtual environment + `requirements.txt`
 **Visualization & Deployment:** Tableau Dashboard and a Webapp deployed via Heroku


### Dataset Details

The system uses a dataset named `Telco-Customer-Churn.csv` which contains information on telecom customers and their key behaviors.

**Features Include:**
 **Demographics:** `gender`, `SeniorCitizen`, `Partner`, `Dependents`
 **Services:** `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`
 **Account Info:** `tenure` (weeks), `Contract`, `PaperlessBilling`, `PaymentMethod`, `MonthlyCharges`, `TotalCharges`
 **Target Variable:** `Churn` (Indicates if the customer stayed or churned)


### Project Structure & Workflow

The repository is organized into a sequential pipeline for reproducibility:

 **`data/`**: Contains raw and processed datasets.
 **`artifacts/`**: Saved train/test splits (`X_train.csv`, `X_test.csv`, etc.).
 **`01_handling_missing_and_duplicate_values.ipynb`**: Data cleaning.
 **`02_handling_outliers.ipynb`**: Statistical outlier management.
 **`03_feature_binning.ipynb`**: Categorizing continuous data.
 **`04_scaling_and_encoding.ipynb`**: Normalization and categorical conversion.
 **`05_model_training.ipynb`**: Model training and evaluation.

**Results**: The Logistic Regression model achieved an **accuracy of 80%** on the test dataset.


