# Customer Churn Analysis (Excel Project)

## Project Overview
This project analyzes telco customer data using Excel to identify drivers of churn and provide actionable insights for retention strategies. 
The analysis focuses on contract types, payment methods, fiber customers, and early lifecycle engagement.

## Dataset
The dataset used for this project is the **IBM Telco Customer Churn dataset** from Kaggle. It contains demographic, account, and usage information for telecom customers, along with churn labels.

- **Source:** Kaggle – [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
- **Content:** Customer demographic information, contract and billing details, usage metrics, and churn indicators.

## Dataset Description
The IBM Telco Customer Churn dataset includes demographic, account, and usage information for telecom customers. Key columns are:

- **customerID** – Unique identifier for each customer  
- **gender** – Customer gender (`Male`/`Female`)  
- **SeniorCitizen** – Indicates if the customer is a senior (0 = No, 1 = Yes)  
- **SeniorStatus** – Added during cleaning to label `SeniorCitizen` as `No`/`Yes` for readability  
- **Partner** – Whether the customer has a partner (`Yes`/`No`)  
- **Dependents** – Whether the customer has dependents (`Yes`/`No`)  
- **tenure** – Number of months the customer has been with the company  
- **PhoneService** – Whether the customer has phone service (`Yes`/`No`)  
- **MultipleLines** – Whether the customer has multiple phone lines (`Yes`/`No`/`No phone service`)  
- **InternetService** – Type of internet service (`DSL`, `Fiber optic`, `No`)  
- **OnlineSecurity** – Whether the customer has online security service (`Yes`/`No`/`No internet service`)  
- **OnlineBackup** – Whether the customer has online backup service (`Yes`/`No`/`No internet service`)  
- **DeviceProtection** – Whether the customer has device protection service (`Yes`/`No`/`No internet service`)  
- **TechSupport** – Whether the customer has technical support service (`Yes`/`No`/`No internet service`)  
- **StreamingTV** – Whether the customer has streaming TV service (`Yes`/`No`/`No internet service`)  
- **StreamingMovies** – Whether the customer has streaming movies service (`Yes`/`No`/`No internet service`)  
- **Contract** – Customer contract type (`Month-to-month`, `One year`, `Two year`)  
- **PaperlessBilling** – Whether the customer uses paperless billing (`Yes`/`No`)  
- **PaymentMethod** – Customer payment method (`Electronic check`, `Mailed check`, `Bank transfer`, `Credit card`)  
- **MonthlyCharges** – The amount charged to the customer monthly  
- **TotalCharges** – The total amount charged to the customer  
- **Churn** – Whether the customer has churned (`Yes`/`No`)  

## Goals
- Identify high-risk customer segments  
- Quantify churn drivers  
- Provide actionable recommendations to reduce churn  

## Key Insights
- **Contract Type:** Month-to-Month customers have a churn rate of **88.55%**, while 1-Year and 2-Year contract customers churn at a minimal rate. 
- **Payment Method:** Electronic Check users show the highest churn rate (57%) compared to other payment methods.  
- **Fiber Customers:** Customers with Fiber service have higher monthly charges compared to other service types, which may contribute to their higher churn rates.
- **Tenure:** Most churn occurs within the first few months of the customer lifecycle, highlighting a critical early engagement period.  

## Recommendations
- **Contract Type:** Promote 1-Year and 2-Year plans with incentives to reduce reliance on Month-to-Month contracts.  
- **Payment Method:** Improve onboarding and communication for Electronic Check users to lower churn risk.  
- **Fiber Customers:** Investigate satisfaction drivers and address complaints to improve retention.  
- **Tenure Building:** Implement early-life cycle engagement initiatives during the first few months to reduce early churn.

  
## Files
[Dashboard View](Telco_Dashboard.png)

[Download The Full Excel Analysis](Telcom_Churn_Insights_Project.xlsx)

## Tools
- Microsoft Excel (with formulas, charts, slicers and pivot tables)  
  

