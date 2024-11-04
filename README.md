# 🧠 **CUSTOMER CHURN PREDICTION** 🚀

---

## 📋 **OVERVIEW**
> ### **Predicting customer churn using machine learning and providing actionable insights for customer retention strategies.**  
> Our model analyzes customer demographics, account information, and service usage patterns to identify those at risk of churning. The solution includes an **interactive Power BI dashboard** and a **deployable API** compatible with web and mobile applications.

---

## 📑 **TABLE OF CONTENTS**
1. [🔍 PROJECT OVERVIEW](#project-overview)
2. [⭐ FEATURES](#features)
3. [📊 DATA](#data)
4. [⚙️ INSTALLATION](#installation)
5. [🚀 USAGE](#usage)
6. [🔧 MODEL TRAINING](#model-training)
7. [📈 DASHBOARD AND API](#dashboard-and-api)
8. [👥 CONTRIBUTORS](#contributors)

---

## 🔍 **PROJECT OVERVIEW**
Customer churn is a significant factor impacting business **revenue and customer satisfaction**. This project provides a **predictive model** to help businesses identify customers at risk, enabling proactive retention strategies.

---

## ⭐ **FEATURES**
- **Data-Driven Insights**: The model evaluates factors contributing to churn, such as contract type, tenure, and support services.
- **Power BI Dashboard**: An interactive dashboard to visualize churn drivers and trends.
- **API Deployment**: A Flask API enables real-time churn predictions, easily integrated into web and mobile applications.

---

## 📊 **DATA**

### Dataset
We used the **Telco Customer Churn** dataset, which includes:
- **Customer Demographics**: gender, senior citizen status, partner, dependents.
- **Service Usage**: phone service, multiple lines, internet service, online security, tech support.
- **Account Information**: contract type, payment method, monthly charges, tenure.

### Target Variable
- **Churn**: A binary variable indicating if a customer has churned ("Yes") or not ("No").

---

## ⚙️ **INSTALLATION**

1. **Clone this repository**:
   ```bash
   git clone https://github.com/yourusername/customer-churn-prediction.git
Install dependencies:
bash
Copy code
pip install -r requirements.txt
🚀 USAGE
1. Data Preprocessing and Model Training
Notebook: Run churn_model_training.ipynb to see the steps for data preprocessing, feature engineering, and model selection.
Pre-trained Model: Use the provided model (customer_churn_model.pkl) for immediate predictions.
2. Power BI Dashboard
Dashboard File: Access it in the /dashboard directory.
Power BI Desktop: Open it for an interactive view of customer churn data.
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
📱 Mobile Accessibility
The API is optimized for mobile compatibility, providing real-time access to churn insights on mobile devices.

🔧 MODEL TRAINING
The model was trained using a subset of customer features, focusing on accuracy and interpretability.

Model Details
Preprocessing: Encoded categorical variables; scaled numerical features.
Algorithm: Model selection based on precision, recall, and F1-score metrics.
📈 DASHBOARD AND API
Power BI Dashboard: Easily interpretable visuals of key churn factors.
Flask API: Real-time predictions through a RESTful API, accessible on web and mobile.
#👥 **CONTRIBUTORS**
Mohamed Hamisa - Machine Learning Engineer
Ahmed Khalid - Data Engineer
Shrouk Sobhy - Machine Learning Engineer
