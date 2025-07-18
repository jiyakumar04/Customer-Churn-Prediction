# **Customer_Churn_Prediction – Banking Domain**

## **Project Overview**
Customer churn is a critical challenge in the banking industry. This project uses machine learning to predict whether a customer will leave (churn) based on demographic and account-related features. The aim is to help banks identify high-risk customers early and implement targeted retention strategies.

---

## **Dataset**
- **Source:** Churn Modelling Dataset (Kaggle)
- **Records:** 10,000+ customers
- **Features:**
  - Demographics: Geography, Gender, Age
  - Account Details: Tenure, Balance, Number of Products, Credit Card, Activity Status
  - Target: `Exited` (1 = Churned, 0 = Retained)

---

## **Key Steps**
1. **Exploratory Data Analysis (EDA):**
   - Churn distribution by age, geography, gender, tenure, and products.
   - Correlation heatmap to understand feature relationships.
2. **Feature Engineering:**
   - Age groups (`18–30`, `31–40`, etc.)
   - High-value customers (balance above median)
   - Active-credit interaction (`IsActiveMember` × `HasCrCard`)
3. **Model Building:**
   - Compared Logistic Regression, Random Forest, and XGBoost.
   - Used ROC-AUC, precision, recall, and F1-score for evaluation.
4. **Explainability:**
   - SHAP values used to identify features most influencing churn.

---

## **Results**
- **Best Model:** XGBoost with **ROC-AUC ≈ 0.87**.
- **Key Drivers of Churn:**
  - Low tenure (new customers)
  - Low activity levels
  - Fewer products held
  - Specific high-churn geographies
- **Business Impact:**
  - Insights can guide retention strategies and reduce churn, saving significant acquisition costs.

---

## **Visuals**
Include key plots:
- Churn distribution  
- Churn by age group and geography  
- SHAP feature importance plots  

---

## **Next Steps**
- Deploy a **Streamlit app** for real-time churn prediction.
- Monitor model performance on new data.
- Integrate customer service interactions and transaction data for improved accuracy.

---

## **How to Run**
1. Clone the repo.
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
pip install -r requirements.txt

