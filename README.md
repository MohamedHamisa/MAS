

Customer Churn Prediction
Overview
This project aims to predict customer churn using machine learning and provide actionable insights to enhance customer retention strategies. The model utilizes a dataset containing customer demographics, account information, and service usage patterns to identify customers at risk of churning. The solution is accessible through an interactive Power BI dashboard and a deployable API, both designed to be integrated into web and mobile applications.

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
Customer churn can significantly impact a business's revenue and customer satisfaction levels. This project addresses this challenge by developing a predictive model to identify potential churn risks, enabling companies to implement proactive retention measures.

Features
Data-Driven Insights: The model evaluates key factors contributing to churn, such as contract type, tenure, and support services.
Power BI Dashboard: An interactive dashboard visualizes churn drivers and trends, providing data insights that are accessible and actionable.
API Deployment: A Flask API allows for real-time churn predictions, making integration into web and mobile applications straightforward.
Data
We used the Telco Customer Churn dataset, which contains:
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
Data Preprocessing and Model Training
Run the notebook churn_model_training.ipynb to explore data preprocessing, feature engineering, and model selection steps.
A pre-trained model (customer_churn_model.pkl) is available for immediate use.
Power BI Dashboard
Our Power BI dashboard provides an interactive view of customer churn data and enables users to filter and analyze churn drivers.

Access the dashboard file in the /dashboard directory.
Open it in Power BI Desktop for further customization and use.
API Deployment
Our API, built with Flask, enables churn predictions on new customer data.

Run the API locally:
bash
Copy code
python app.py
API Endpoint: /predict_churn
Example JSON Input:
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
The API is compatible with mobile devices, allowing real-time access to churn insights on the go.

Model Training
The model was trained on a subset of customer features, focusing on accuracy and interpretability. Various models were tested, and the final model was selected based on optimal performance across multiple metrics.

Model Details
Preprocessing: Categorical variables were encoded, and numerical features were scaled.
Algorithm: The model was chosen based on its precision, recall, and F1-score.
Dashboard and API
Our solution includes:

Power BI Dashboard: Visualizes key churn factors in an intuitive way.
Flask API: Provides real-time predictions via a RESTful API, accessible on web and mobile.
Contributors
Mohamed Hamisa - Machine Learning Engineer
Ahmed Khalid - Data Engineer
Shrouk Sobhy - Machine Learning Engineer
