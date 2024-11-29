# Churn Prediction Project
This project predicts customer churn using an artificial neural network (ANN) model trained on a dataset with features such as geography, gender, age, balance, credit score, tenure, number of products, has credit card, isActiveMember, estimated salary, and exit status. After thorough preprocessing, including feature scaling and encoding, the ANN model was developed to classify customers as likely to churn or retain. The solution is deployed on Streamlit Cloud, providing a user-friendly interface for real-time churn predictions, enabling businesses to implement proactive retention strategies.

## Table of Contents:
1. Project Overview <br>
2. Generated project structure <br>
3. Dataset Information <br>
4. Project Workflow <br>
5. Installation <br>
6. Usage <br>
7. Model Development <br>
8. Evaluation <br>
9. Results <br>
10. Contributing <br>
11. License <be>


## Project Overview:
**Problem Statement:**
Predict whether a customer is likely to churn and estimate their salary.

**Goal:**
By estimating customer salary, the bank can target potential customers for loans, increasing business opportunities. Predicting customer churn enables the bank to take proactive measures to retain customers and reduce churn rates.

**Solution:**
An Artificial Neural Network (ANN) model is used to train and predict both churn likelihood and customer salary


## Generated Project Structure:
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
├── logs/                           # Classification specific logs
│   ├── train/                      # Training logs
│   └── validation/                 # Validation logs
│
├── regression_logs/                # Regression-specific logs
│   ├── train/                      # Training regression logs
│   └── validation/                 # Validation regression logs
│
├── models/                         # Saved models
│   ├── models.h5                   # Classification model file
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


## Dataset Information: <br>
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

## Project Workflow:

- **Data Collection:**  
  The dataset was obtained from Kaggle as the primary resource.

- **Data Preprocessing:**  
  Data preprocessing was performed using the Pandas library in Python, which involved cleaning and transforming the data.

- **Feature Engineering:**  
  Relevant features were selected and engineered to enhance model performance.

- **Model Selection:**  
  Artificial Neural Networks (ANN) were chosen as the model for predicting customer churn and estimating salary.

- **Model Training and Optimization:**  
  The ANN model was trained using the preprocessed data, followed by optimization to improve accuracy and performance.

- **Prediction:**  
  The model predicts both the estimated salary of the customer and whether the customer is likely to churn.

- **Deployment:**  
  The model was deployed on Streamlit Cloud for interactive real-time predictions, and the code was checked into GitHub for version control and contribution tracking.

## Installation:
Provide the steps for setting the environment
# Clone the repository
git clone https: https://github.com/saichakka10/ANN-Churn-Prediction.git

# Change directory
cd ANN-Churn-Prediction

# Create a conda environment
conda create -p venv python==3.11 -y

# Activate conda environment
conda activate venv

# Install required packages
pip install -r requirements.txt

# Deactivate the environment
conda deactivate


## Usage:

### **Experiments:**
The `experiments.ipynb` file is used for data cleaning, preprocessing, splitting the dataset into training and testing sets, and implementing an Artificial Neural Network (ANN) for the classification task. The model predicts whether the customer is likely to churn or not.

### **Prediction:**
The `prediction.ipynb` file is used to make predictions based on the trained classification model. It outputs the likelihood of customer churn.

### **Salary Regression:**
The `salaryregression.ipynb` file is used for data cleaning, preprocessing, splitting the dataset into training and testing sets, and implementing an ANN model for regression. This model predicts the estimated salary of the customer.

## Evaluation:

### **Metrics Used:**

- **Classification:**  
  Accuracy is used as the evaluation metric to measure how well the model classifies customer churn.

- **Regression:**  
  The Mean Absolute Error (MAE) is used to evaluate the regression model's performance in predicting the customer's salary.

## Contributing:

1. Fork the repository.
2. Create a new branch:  
   ```bash
   git checkout -b feature-branch
3. git commit -m 'Add feature'
4. git push origin feature-branch
5. This version is structured with better clarity and consistency, making it easier to read and follow the steps.

## Deployment:

The deployment of the project has been done on **Streamlit Cloud** for enhanced user interaction. The following files are used in the deployment:

- **`app.py`:** This file serves as the main application that provides an interactive user interface. It facilitates the prediction of customer churn, allowing users to input data and view results in real-time.
  
- **`streamlit_regression.py`:** This file specifically handles the regression model used for predicting the customer’s estimated salary. It ensures that users can interact with the model and get immediate predictions.

**Streamlit Cloud** is a cloud-based platform that simplifies the process of deploying and sharing machine learning models as interactive web apps. Streamlit Cloud allows developers to deploy apps directly from a GitHub repository without the need to manage infrastructure. It automatically updates whenever the repository is updated, streamlining deployment and making it easy to share your projects with collaborators or stakeholders.

### Key Features of Streamlit Cloud:
- **Interactive Interface:** Streamlit provides an easy-to-use interface to display data, plots, and real-time predictions.
- **Quick Deployment:** With minimal setup, you can deploy your app directly from GitHub, making it accessible to others instantly.
- **Automatic Updates:** When changes are made to the codebase or GitHub repository, the app is automatically updated without requiring manual intervention.
- **Easy Sharing:** You can share your app with others by simply providing a link, making it ideal for presentations and collaborations.


## License: 
This project is licensed under the MIT License
