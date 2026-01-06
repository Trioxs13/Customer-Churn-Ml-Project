**Customer Churn Prediction – End-to-End Machine Learning Project**

**📌 Project Overview**

Customer churn is one of the most critical challenges for subscription-based businesses, directly impacting revenue, growth, and customer lifetime value.
This project builds a fully end-to-end machine learning solution to predict customer churn using historical customer data, enabling organisations to proactively identify high-risk customers and implement targeted retention strategies.

The project demonstrates the complete machine learning lifecycle — from exploratory data analysis and preprocessing to model training, evaluation, interpretation, and business recommendations.

**🎯 Project Objectives**

Perform exploratory data analysis (EDA) to understand customer behaviour

Identify the key factors that drive customer churn

Build and compare multiple machine learning models

Select the best-performing model using appropriate evaluation metrics

Interpret model results and translate them into actionable business insights

**📂 Dataset**

Dataset: IBM Telco Customer Churn Dataset

Dataset Size:

7,043 customer records

20+ features

Target Variable:

Churn — indicates whether a customer has left the service (Yes / No)

**🔍 Exploratory Data Analysis (EDA)**

Key insights from EDA:

The dataset is imbalanced, with approximately 27% churned customers and 73% non-churned customers

Customers with low tenure (0–6 months) show the highest churn rates

Month-to-month contracts are strongly associated with churn

Customers using fiber optic internet services churn more frequently

Electronic check payment method has a high churn correlation

Customers subscribed to OnlineSecurity and TechSupport churn significantly less

These findings guided feature engineering, model evaluation strategy, and business recommendations.

**🛠 Data Preprocessing**

The following preprocessing steps were applied to prepare the data for modelling:

Converted TotalCharges to numeric and handled missing values

Dropped irrelevant identifier columns (e.g., customerID)

Applied one-hot encoding to categorical variables

Scaled numerical features using StandardScaler

Split the dataset into training and testing sets (80/20 split)

**🤖 Machine Learning Models**

The following machine learning models were trained and evaluated:

1. Logistic Regression

2. Random Forest

3. XGBoost

**Evaluation Metrics**

Because churn prediction involves an imbalanced dataset, evaluation focused on:

Recall (Churn class) — prioritised to capture as many churners as possible

F1-score (Churn class) — balances precision and recall

ROC-AUC — measures overall model discrimination ability

**📊 Model Performance Summary**
Model              	Recall (Churn)	        F1-Score (Churn)	      ROC-AUC
Logistic Regression	0.90	                  0.88                  	0.852
Random Forest	      0.78	                  0.84                  	0.853
XGBoost	            0.91	                  0.88                  	0.855
✅ Final Model Selection

XGBoost was selected as the final model due to its superior ROC-AUC score and strong balance between recall and F1-score. It effectively captures non-linear relationships and complex feature interactions.

**🔑 Feature Importance Analysis (XGBoost)**

Feature importance analysis from the XGBoost model highlights the most influential factors contributing to churn:

InternetService – Fiber optic

Contract type – Month-to-month

Payment method – Electronic check

Customer tenure

Online security and technical support add-ons

Monthly charges

These features align closely with real-world customer behaviour in subscription-based services.

**💡 Business Insights & Recommendations**

- Based on the model insights, the following recommendations can help reduce customer churn:

- Encourage long-term contracts by offering incentives to month-to-month customers

- Improve onboarding and engagement for new customers in the first few months

- Investigate service quality and pricing for fiber optic internet plans

- Promote automatic payment methods instead of electronic checks

- Bundle security and technical support services to improve customer satisfaction

**🧪 Technologies Used**
1.Python
2.Pandas, NumPy
3.Scikit-learn
4.XGBoost
5.Matplotlib, Seaborn
6.Jupyter Notebook
