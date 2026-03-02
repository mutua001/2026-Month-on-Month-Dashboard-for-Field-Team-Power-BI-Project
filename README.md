# 2026-Month-on-Month-Dashboard-for-Field-Team-Power-BI-Project

* 📌 Overview

- This project presents a Power BI dashboard designed for the field team to monitor key performance indicators (KPIs) on a monthly basis. The dashboard focuses on:

- Repayment rates and average daily electricity usage per customer cohort (month)

- Risk segmentation of cohorts based on repayment behavior and usage patterns

 - Arrears distribution and contribution analysis

- Identification of high-risk customers for targeted follow-up

## The analysis covers the first quarter of 2026 (January – March) and provides actionable insights to improve collections and customer engagement.

📁 Repository Structure
text
├── data/                     - Raw and processed data (CSV, Excel)
├── dashboard/                - Power BI .pbix file
├── images/                   - Screenshots of dashboard
├── README.md                 - Project documentation (this file)
├── requirements.txt          - Dependencies (if any)
└── methodology.md            - Detailed steps of analysis
📊 Data Sources

* The data is simulated based on field operations and includes:

* Time period: January – March 2026

* Fields: Customer Name, Month, Amount Paid (KES), Total kWh Used, Rate of Payment (%), Arrears (KES), Active Days

* Note: All data is anonymized and used for demonstration purposes only.

## 🧮 Key Metrics Calculated

-- Repayment Rate (%)

-- Defined as:

-- Repayment Rate = (Amount Paid / Expected Billing) * 100

-- Calculated per customer, then averaged per cohort (month)

-- Average Daily kWh Usage

-- Average Daily Usage = Total kWh Used / Active Days

-- Active days = number of days with recorded usage

-- Overall Portfolio Repayment Rate

-- Weighted average of all monthly repayment rates

-- Overall Average Daily Usage

--- Average of daily usage across all customers

--Arrears Contribution (%)

-- Arrears Contribution = (Sum of Arrears in Month / Total Portfolio Arrears) * 100
📈 Dashboard Design

##The dashboard consists of the following pages:

###Page 1: Executive Summary

##KPI Cards

##Total Amount Paid: 39,000 KES

##Total kWh Used: 781.4 kWh

##Average Repayment Rate: 49.5% (from monthly averages)

##Total Arrears: 31,000 KES

###Monthly Trends (Line/Bar Charts)

###Amount Paid by Month

###Average Repayment Rate by Month

###Total kWh Used by Month

###Arrears by Month

##Page 2: Cohort & Risk Analysis

###Repayment Rate by Month

###Jan: 31.11%

##Feb: 52.35%

##Mar: 65.19%

##Average Daily Usage by Month

###Jan: 56.2 kWh

###Feb: 83.0 kWh

##Mar: 97.0 kWh

##Risk Segmentation Table

##Month	Repayment Rate	Avg Daily Usage	Risk Tier
##Jan	31.11%	56.2 kWh	High
##Feb	52.35%	83.0 kWh	Medium
##Mar	65.19%	97.0 kWh	Medium

###Note: March’s high usage pushes it toward High, but repayment is improving.

##Page 3: Arrears Deep Dive

###Arrears Distribution by Month (Pie Chart)

###Contribution Percentages:

###Jan: 16.1% (5,000 / 31,000)

###Feb: 48.4% (15,000 / 31,000)

###Mar: 35.5% (11,000 / 31,000)

###Top 10 Customers with Highest Arrears

###Highlights high-risk individuals for follow-up

###Page 4: High-Risk Customers

###List of customers flagged as high-risk (based on risk tiers)

###Their individual arrears, repayment rate, and usage

###Drill-through to customer details

##⚠️ Risk Segmentation

##Cohorts (months) are classified into Low, Medium, or High risk using two dimensions:

##Repayment Rate (lower is riskier)

##Average Daily Usage (higher may indicate potential overuse or inability to pay)

##Threshold Justification:

###Low Risk: Repayment ≥ 80% AND daily usage < 50 kWh

###Customers paying well and consuming modestly

###Medium Risk: Repayment between 50–80% OR daily usage between 50–100 kWh

###Moderate performance; needs monitoring

###High Risk: Repayment < 50% OR daily usage > 100 kWh

###Poor payment or excessive consumption, likely to default

##📉 Arrears Analysis

##Total Portfolio Arrears: 31,000 KES

###February: Largest share, 48.4%, driven by a few large defaults

###January: Smallest arrears but lowest repayment rate, possible write-offs or recent defaults

###Arrears by Month

##Jan: 5,000 KES (16.1%)

##Feb: 15,000 KES (48.4%)

##Mar: 11,000 KES (35.5%)

###🔍 Additional Insights

###Seasonality: Repayment rates improved from Jan → Mar, possibly due to better collection efforts or economic factors

###Usage Spike in March: Average daily usage rose to 97 kWh, potentially stressing repayment capacity

###High-Risk Customers: e.g., Alifred Joseph, Brian Njoroge have arrears > 2,000 KES and repayment rates < 30%. Immediate follow-up recommended

##💡 Data-Driven Recommendations

###Target February Cohort for Intensive Collection

###Feb has highest arrears (15,000 KES) and medium risk

###Deploy field agents with customized payment plans

###Introduce Usage Alerts for Customers Exceeding 80 kWh/day

###High usage correlates with higher default risk

###Send SMS alerts with energy-saving tips or flexible payment options

###Reward Consistent Payers in March Cohort

###March achieved highest repayment rate (65%) despite high usage

###Consider loyalty discounts or priority maintenance

###Quantitative Basis:

###Feb arrears = 15,000 KES; repayment rate = 52% → room for improvement

###Average daily usage in high-risk months > 80 kWh

###March repayment rate improved by 34 percentage points from January
