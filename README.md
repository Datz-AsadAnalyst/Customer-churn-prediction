# 🔍 Customer Churn Prediction 
## Objective:
Predict customer churn for a telecom company using Machine learning model and identify key factors contributing to churn.

## 📁 Dataset Overview
- Source: Public telecom dataset
- Rows: 7,000+
- Target Variable: Churn (Yes/No)
## Key Features Used:
- TotalCharges
- tenure
- MonthlyCharges
- Contract_Two year
- InternetService_Fiber optic

## 🧱 Steps Followed
### 1. 📊 Data Preprocessing
- Handled missing values and data types (e.g., converted TotalCharges from object to float)

- Encoded categorical features using one-hot encoding

- Scaled numerical features using StandardScaler

### 2. ✂️ Train-Test Split
- Stratified split: 80% training, 20% testing

### 3. ⚖️ Class Balancing
- Compared performance with and without class weights
- Tested SMOTE but found balanced class weight yielded better results in logistic regression

### 4. 🧠 Modeling
- Primary model: **Logistic Regression**
- Secondary models tested: **Random Forest**, **XGBoost**

### 5. 📈 Evaluation
- Accuracy: ~77%
- Precision (Class 1): ~0.56
- Recall (Class 1): ~0.61
- ROC AUC: 0.81

### 6. 🔍 Feature Importance
- Extracted top 5 most influential features using sklearn model coefficients.

## 🎯 Key Insights
- Customers with high TotalCharges and MonthlyCharges are more likely to churn.
- Short tenure is a strong indicator of churn.
- Customers on Fiber optic internet and Month-to-month contracts are at higher risk.

## 📂 Files
- churn_cleaned.csv — Cleaned dataset
- churn_model.ipynb — Full notebook with EDA, feature engineering, modeling, and evaluation
- models/ — Trained model files
- README.md — Project summary

## 🚀 Future Work
- Implement more advanced ensemble methods
- Deploy as a web app using Streamlit
- Perform customer segmentation using clustering

## 🧠 Author
Asad Ali  Data Scientist & Visualization Specialist

LinkedIn | Portfolio | Email

