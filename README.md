                     **Bank Risk Intelligence Dashboard**

An end-to-end bank risk analytics platform built using Microsoft Fabric and Power BI Service.

## Overview
This project simulates a retail banking risk intelligence system analyzing a $513M loan portfolio across 1,000 customers, 2,000 loans, and 5,000 transactions.

## Tech Stack
- Microsoft Fabric Lakehouse (data storage)
- Power BI Service (report building)
- DAX (measures and calculations)
- Star Schema Data Model

## Data Model
7 tables with star schema design:
- fact_loans (2,000 rows)
- fact_deposits (2,000 rows)
- fact_transactions (5,000 rows)
- fact_credit_risk (2,000 rows)
- dim_customer (1,000 rows)
- dim_product (10 rows)
- dim_date (2,192 rows)

## Report Pages
1. Executive Summary — KPIs, segment analysis, deposit mix
2. Loan Portfolio Analysis — loan status, product breakdown, tenure
3. Deposits & Customer Analysis — deposit trends, credit scores
4. Fraud Analysis — fraud rate (3.19%), channel & segment breakdown
5. Credit Risk Analysis — ECL ($26.97M), RWA ($199.96M)

## Key DAX Measures
- Expected Credit Loss: ECL = PD × LGD × EAD (Basel III)
- NPA Rate, Fraud Rate, Delinquency Rate
- Average Credit Score, Total RWA

## Features
- Synced slicers across all 5 pages
- Conditional formatting on all charts
- Executive dashboard with pinned KPIs
- Interactive filtering by segment, loan status, product, channel, risk grade
