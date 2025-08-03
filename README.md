# ANN-EstimatedSalaryPrediction-Regression

# Customer Estimated Salary Predictor

This project uses an Artificial Neural Network (ANN) regression model to predict a customer's estimated salary based on their banking information and demographic data. The model is deployed as an interactive web application using Streamlit.

## Live Application

**You can access the live deployed application here:**

[**➡️ Live Salary Predictor App**](https://mxxgaxfyxqdzg24d2d2kn2.streamlit.app/) 


## Project Overview

The core of this project is a regression model trained to find a relationship between a customer's profile and their likely salary. This can be useful for targeted marketing, financial product recommendations, and understanding a bank's customer base.

## Dataset

The model is trained on the "Churn_Modelling.csv" dataset. The following features are used as inputs for the prediction:

* CreditScore
* Geography
* Gender
* Age
* Tenure
* Balance
* NumOfProducts
* HasCrCard
* IsActiveMember
* Exited (Whether the customer has previously churned)

The target variable for the prediction is **EstimatedSalary**.

## Model and Preprocessing

* **Model**: An Artificial Neural Network built with TensorFlow and Keras, designed for regression tasks. The output layer produces a single continuous value representing the predicted salary.
* **Preprocessing**:
    * **Label Encoding**: The `Gender` feature is converted from text to a numerical format.
    * **One-Hot Encoding**: The categorical `Geography` feature is converted into numerical columns.
    * **Feature Scaling**: All input features are standardized using `StandardScaler` to ensure the model performs optimally.

## Interactive Web Application

A user-friendly web application, built with Streamlit, serves as the frontend for the model. It allows users to:
* Input all the required customer details using sliders, dropdowns, and number inputs.
* Submit the data to the trained regression model.
* Receive an instant prediction of the customer's estimated salary.

## How to Run the Project Locally

1.  **Clone the repository**:
    ```bash
    git clone [[https://github.com/chaitanyananepallicn/ANN-Customer-Churn-Predictor.git](https://github.com/chaitanyananepallicn/ANN-Customer-Churn-Predictor.git)](https://github.com/chaitanyananepallicn/ANN-EstimatedSalaryPrediction-Regression-.git)
    ```
    
3.  **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

2.  **Navigate to the project directory**:
    ```bash
    cd ANN-Customer-Churn-Predictor
    ```

4.  **Run the Streamlit application**:
    ```bash
    streamlit run ChurnModeling-ANN/app.py
    ```
5.  Open your web browser and navigate to the local URL provided by Streamlit.

