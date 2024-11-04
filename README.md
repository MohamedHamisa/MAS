
**Customer Churn Prediction
Overview
This project aims to predict customer churn using machine learning and provide actionable insights for customer retention strategies.
Our model uses customer demographics, account information, and service usage patterns to identify customers at risk of churning. The solution includes an interactive Power BI dashboard and a deployable API compatible with web and mobile applications.

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
Customer churn can significantly impact a business’s revenue and customer satisfaction. This project provides a predictive model to help businesses identify customers at risk of churning, enabling proactive retention strategies.

Features
Data-Driven Insights: The model evaluates factors contributing to churn, such as contract type, tenure, and support services.
Power BI Dashboard: An interactive dashboard to visualize churn drivers and trends, making data actionable.
API Deployment: A Flask API enables real-time churn predictions, easily integrated into web and mobile applications.
Data
Dataset
We used the Telco Customer Churn dataset, containing information on:

Customer Demographics: gender, senior citizen status, partner, dependents.
Service Usage: phone service, multiple lines, internet service, online security, tech support.
Account Information: contract type, payment method, monthly charges, and tenure.
Target Variable
Churn: A binary variable indicating if a customer has churned ("Yes") or not ("No").
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
Notebook: Run churn_model_training.ipynb to see the steps taken for data preprocessing, feature engineering, and model selection.
Pre-trained Model: Use the pre-trained model (customer_churn_model.pkl) for immediate predictions.
2. Power BI Dashboard
Dashboard File: Access the file in /dashboard directory.
Power BI Desktop: Open it for a detailed, interactive view of customer churn data.
3. API Deployment
Run the API locally:
bash
Copy code
python app.py
API Endpoint: /predict_churn
Sample Input:
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
The API is optimized for mobile compatibility, enabling real-time access to churn insights on mobile devices.

Model Training
The model was trained using a subset of customer features, prioritizing accuracy and interpretability.

Model Details
Preprocessing: Categorical variables were encoded; numerical features were scaled.
Algorithm: Model selection was based on precision, recall, and F1-score metrics.
Dashboard and API
Power BI Dashboard: Visualizes key churn factors, making data understandable and actionable.
Flask API: Real-time predictions through a RESTful API, accessible on web and mobile.
Contributors
Mohamed Hamisa - Machine Learning Engineer
Ahmed Khalid - Data Engineer
Shrouk Sobhy - Machine Learning Engineer
