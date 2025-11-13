# Customer Churn Analysis (Excel Project)

## Project Overview
This project analyzes telco customer data using Excel to identify drivers of churn and provide actionable insights for retention strategies. 
The analysis focuses on contract types, payment methods, fiber customers, and early lifecycle engagement.

## Dataset Source
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

## Data Cleaning and Preparation
Before performing the analysis, the following steps were applied to the IBM Telco dataset:

1. **Senior Status Column:** Added a `SeniorStatus` column to label `SeniorCitizen` as `Yes` or `No` for better readability.  
2. **Missing Values:** Deleted rows where `MonthlyCharges` were missing  and `tenure` was 0, since these correspond to new customers who have not yet been billed and are not relevant for churn analysis.  
3. **Consistency Checks:** Ensured categorical fields (`Yes`/`No`) are consistent, and numeric fields are correctly formatted.  
4. **Focus Columns:** Verified that all relevant columns for churn analysis (contract, payment method, internet service, tenure, monthly charges, churn) were properly formatted and ready for calculation.  

---

 ##  Explore the Data 
   - The uploaded workbook (`Telco_Churn_Insights_Project.xlsx`) contains all sheets used for this project in one file, including:  
     - **Original dataset sheet**  
     - **Cleaned dataset sheet**  
     - **KPIs sheet** (with the formulas used to calculate key metrics)  
     - **Analysis sheet** (with pivot tables + charts)  
     - **Insight sheet** (where key findings were summarised)  
   - You can open this Excel file and interact directly with slicers, pivot tables, and KPIs to explore the churn patterns dynamically.

## Analysis Methodology
Key KPIs were calculated using Excel formulas on the cleaned dataset and stored in a sheet named KPIS.

- **Churn Rate:**  
`=(COUNTIF(cleaned!U2:U7033, "Yes") / COUNTA(cleaned!A2:A7033)) * 100`  
Calculates the percentage of customers who churned.

- **MRR by Active Customers:**  
`=SUMIF(cleaned!U2:U7033, "No", cleaned!S2:S7033)`  
Sums the monthly charges for all active (non-churned) customers.

- **Average Tenure of Churned Customers:**  
`=AVERAGEIF(cleaned!U2:U7033, "Yes", cleaned!F2:F7033)`  
Computes the average tenure for customers who have churned.

- **Average Tenure of Non-Churned Customers:**  
`=AVERAGEIF(cleaned!U2:U7033, "No", cleaned!F2:F7033)`  
Computes the average tenure for customers who are still active.

Pivot tables, charts, and slicers (e.g., Gender, SeniorStatus) were then used to dynamically explore the data and visualize key insights. Finally, a dashboard was built to summarize findings interactively.


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
[Dashboard Image View](Telco_Churn_Dashboard.png)

[Dashboard Video View](Telco_Churn_Clip.gif)

[Download The Full Excel Analysis](Telco_Churn_Insights_Project.xlsx)

## Tools
- Microsoft Excel (with formulas, charts, slicers and pivot tables)

## Topics / Tags
#excel #powerbi #dataanalysis #telecom #customerchurn #dashboard #analytics #kpi

## Contact
If you would like to connect or have questions about this analysis, reach out:

- LinkedIn:[my linkdn](https://www.linkedin.com/in/linet-rono-b32130277/)
- Email: [my email](mukamihrono@gmail.com)

## Reuse
This project is open for learning purposes —  
you are welcome to reference, adapt or build on this work in your own projects.

Please credit or reference this repository if you use any parts of it.

  

