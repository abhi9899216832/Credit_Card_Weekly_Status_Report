# Credit_Card_Weekly_Status_Report (Interactive Dashboard Creating usding power-bi and MySQL)
## Project Objective
To develop a comprehensive credit card weekly dashboard that provides real-time insights into key performance metrics and trends, enabling stakeholders to monitor and analyze credit card operations effectively.

## DataSet Used
<a href="https://github.com/abhi9899216832/Credit_Card_Weekly_Status_Report/blob/main/credit_card.csv">Credit card file</a> <br>
<a href="https://github.com/abhi9899216832/Credit_Card_Weekly_Status_Report/blob/main/customer.csv">Customer file</a>

## After completing the Dashboard more data to add in our Dataset.
<a href="https://github.com/abhi9899216832/Credit_Card_Weekly_Status_Report/blob/main/cc_add.csv">Credit Card add</a><br>
<a href="https://github.com/abhi9899216832/Credit_Card_Weekly_Status_Report/blob/main/customer.csv">Customer add</a>
<br>
## Credit card financial dashboard using Power BI:
- Developed an interactive dashboard using transaction and customer data from a SQL database, to provide real-time insights. 
- Streamlined data processing & analysis to monitor key performance metrics and trends.
- Shared actionable insights with stakeholders based on dashboard findings to support decision-making processes.

# Project Insights- Week 53 (31st Dec)
## WoW change: 
- Revenue increased by 28.8%, 
- Total Transaction Amt & Count increased by xx% & xx%
- Customer count increased by xx%
## Overview YTD:
- Overall revenue is 57M
- Total interest is 8M
- Total transaction amount is 46M
- Male customers are contributing more in revenue 31M, female 26M
- Blue & Silver credit card are contributing to 93% of overall 
## transactions
- TX, NY & CA is contributing to 68%
- Overall Activation rate is 57.5%
- Overall Delinquent rate is 6.06%


# Charts
- I used KPI cards in my dashboard with is represent beautifully to show Revenue, Income, Interest, Customer satisfaction result.
- I used slicer also to indicate the like a button with we click one of them they show a result according to Q1, Q2, Q3, Q4 THIS SHOW'S IN QUATER RESULTS.
- I used bar charts, line chart and table also.

# This is Credit Card Customer Report
<img width="608" height="344" alt="Screenshot_Credit_Card_Customer_Report" src="https://github.com/user-attachments/assets/fbcc1302-e1f4-4a55-a3d1-fd9a5ef36c52" />

# Credit Card Transaction Report
<img width="609" height="344" alt="Screenshot_Credit_Card_Report" src="https://github.com/user-attachments/assets/0ea795f0-bf4b-46be-a8c5-327e1d52b4e8" />


# DAX Queries
AgeGroup = SWITCH(
TRUE(),
'public cust_detail'[customer_age] < 30, "20-30",
'public cust_detail'[customer_age] >= 30 && 'public cust_detail'[customer_age] < 40, "30-40",
'public cust_detail'[customer_age] >= 40 && 'public cust_detail'[customer_age] < 50, "40-50",
'public cust_detail'[customer_age] >= 50 && 'public cust_detail'[customer_age] < 60, "50-60",
'public cust_detail'[customer_age] >= 60, "60+",
"unknown"
)
IncomeGroup = SWITCH(
TRUE(),
'public cust_detail'[income] < 35000, "Low",
'public cust_detail'[income] >= 35000 && 'public cust_detail'[income] <70000, "Med",
'public cust_detail'[income] >= 70000, "High",
"unknown"
)

# Project Conclusion (Points)
- Successfully developed a Credit Card Financial Weekly Dashboard using Power BI.
- Integrated and processed data from SQL database for accurate analysis.
- Used DAX formulas to create calculated columns like revenue, age group, and income group.
- Dashboard provides real-time insights into revenue, transactions, and customer behavior.
- Identified key trends such as increase in weekly revenue and transaction activity.
- Highlighted important business metrics like activation rate and delinquency rate.
- Enabled better decision-making by presenting clear and interactive visualizations.
- The project demonstrates strong skills in data analysis, data visualization, and business intelligence.
