# Churn Prediction Project
This project predicts customer churn using an artificial neural network (ANN) model trained on a dataset with features such as geography, gender, age, balance, credit score, tenure, number of products, has credit card, isActiveMember, estimated salary, and exit status. After thorough preprocessing, including feature scaling and encoding, the ANN model was developed to classify customers as likely to churn or retain. The solution is deployed on Streamlit Cloud, providing a user-friendly interface for real-time churn predictions, enabling businesses to implement proactive retention strategies.

Table of Contents:
1. Project Overview <br>
2. Dataset Information <br>
3. Project Workflow <br>
4. Installation <br>
5. Usage <br>
6. Model Development <br>
7. Evaluation <br>
8. Results <br>
9. Contributing <br>
10. License <be>


Problem Statement:
Predict whether a customer is likely to churn and estimate their salary.

Goal:
By estimating customer salary, the bank can target potential customers for loans, increasing business opportunities. Predicting customer churn enables the bank to take proactive measures to retain customers and reduce churn rates.

Solution:
An Artificial Neural Network (ANN) model is used to train and predict both churn likelihood and customer salary


Dataset Information:<br>
**Credit Score:** The customer's credit score, which reflects their creditworthiness.<br>
**Geography:** The geographic region where the customer resides (Spain, France, Germany).<br>
**Gender:** The gender of the customer (Male or Female).<br>
**Age:** The age of the customer.<br>
**Tenure:** The length of time the customer has been with the bank.<br>
**Balance:** The current bank balance of the customer.<br>
**Number of Products:** The total number of products the customer uses with the bank.<br>
**Has Credit Card:** Whether or not the customer holds a credit card with the bank.<br>
**Is Active Member:** Indicates how actively the customer is using the bank's services.<br>
**Estimated Salary:** The estimated annual salary of the customer.<br>
**Exited:** Whether or not the customer is likely to churn (exit the bank).<br>


Generated Project Structure
<pre>
project_name/
│
├── data/                           # Data-related files
│   ├── raw/                        # Raw, unprocessed data files
│   └── processed/                  # Processed data files (if applicable in the future)
│
├── notebooks/                      # Jupyter notebooks for EDA and experimentation
│   ├── experiments.ipynb           # Experimentation notebook
│   ├── prediction.ipynb            # Prediction notebook
│   └── salaryregression.ipynb      # Salary regression notebook
│
├── pickle/                         # Pickle files for preprocessing
│   ├── label_encoder_gender.pkl    # Label encoder for gender
│   ├── onehot_encoder_geo.pkl      # One-hot encoder for geographical data
│   └── scaler.pkl                  # Scaler for normalization
│
├── logs/                           # Logs for general processes
│   ├── train/                      # Training logs
│   └── validation/                 # Validation logs
│
├── regression_logs/                # Regression-specific logs
│   ├── train/                      # Training regression logs
│   └── validation/                 # Validation regression logs
│
├── models/                         # Saved models
│   ├── models.h5                   # Main model file
│   └── regression_model.h5         # Regression model file
│
├── reports/                        # Reports and visualizations
│   └── figures/                    # Plots and visualizations
│
├── app.py                          # Main application script
├── streamlit_regression.py         # Streamlit app for the regression model
├── requirements.txt                # Dependencies and libraries
├── README.md                       # Project overview
└── .gitignore                      # Git ignore file
</pre>


License: This project is licensed under MIT License
