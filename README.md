

Customer Churn Prediction
Overview
This project aims to predict customer churn using machine learning and provide actionable insights for retention strategies. Our model leverages a dataset of customer demographics, account information, and service usage patterns to identify customers at risk of leaving. The solution is designed to be accessible, with an interactive Power BI dashboard and a deployable API that allows for easy integration into applications, including mobile.

Table of Contents
Project Overview
Features
Data
Installation
Usage
Model Training
Dashboard and API
Contributors
Project Overview
Customer churn can have a significant impact on revenue and customer satisfaction. This project provides a predictive model that helps businesses identify potential churn risks and take proactive measures to retain customers.

Features
Data-Driven Insights: The model evaluates key factors that contribute to churn, including contract type, tenure, and support services.
Power BI Dashboard: An interactive dashboard visualizes churn drivers and trends, making data accessible and actionable.
API Deployment: A Flask API enables real-time churn predictions, making it easy to integrate into web or mobile applications.
Data
We used the Telco Customer Churn dataset, which contains information on:

Customer Demographics: gender, senior citizen status, partner, and dependents.
Service Usage: phone service, multiple lines, internet service, online security, and tech support.
Account Information: contract type, payment method, monthly charges, and tenure.
Target Variable
Churn: Binary variable indicating if a customer has churned (Yes) or not (No).
Installation
Clone this repository:
bash
Copy code
git clone https://github.com/yourusername/customer-churn-prediction.git
Install dependencies:
bash
Copy code
pip install -r requirements.txt
Usage
1. Data Preprocessing and Model Training
To prepare the data and train the model:

Run the notebook churn_model_training.ipynb to see the steps taken for data preprocessing, feature engineering, and model selection.
A pre-trained model (customer_churn_model.pkl) is provided for immediate use.
2. Power BI Dashboard
Our Power BI dashboard provides an interactive view of customer churn data and allows users to filter and explore churn drivers.

Access the dashboard file in the /dashboard directory.
Open it in Power BI Desktop for further customization and use.
3. API Deployment
Our API, built with Flask, allows for churn predictions on new customer data.

Run the API locally with:
bash
Copy code
python app.py
The /predict_churn endpoint takes JSON input and returns a prediction indicating whether a customer is likely to churn.
Example JSON input:

json
Copy code
{
    "num__tenure": 12,
    "num__MonthlyCharges": 50.30,
    "cat__PaymentMethod": "Electronic check",
    "cat__Contract_TwoYear": 0,
    "cat__OnlineSecurity_Yes": 0,
    "cat__TechSupport_Yes": 1,
    "cat__MultipleLines_Yes": 1,
    "cat__InternetService_Fiber": 1
}
Mobile Accessibility
The API is compatible with mobile devices, enabling easy integration for real-time access to churn insights on the go.

Model Training
The model was trained on a subset of customer features with a focus on accuracy and interpretability. We evaluated different models, choosing the one with the best balance of performance and precision.

Model Details:
Preprocessing: Categorical variables were encoded, and numerical features were scaled.
Algorithm: The final model was chosen based on a range of metrics, including precision, recall, and F1-score.
Dashboard and API
Our solution includes:

Power BI Dashboard: Easily interpretable visuals of key churn factors.
Flask API: Real-time predictions via a RESTful API that’s accessible on web and mobile.
Contributors
Mohamed Hamisa - Machine Learning Engineer
Ahmed Khalid - Data Engineer
Shrouk Sobhy - Machine Learning Engineer
