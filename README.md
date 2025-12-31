# 💰 Loan Data ETL & Analytics Pipeline

**AlmaBetter Verified • PostgreSQL + Excel Dashboard • 70K+ Bank Loan Records • Nov 2025**

<img width="962" height="922" alt="Dashboard" src="https://github.com/user-attachments/assets/3f46dda9-b221-4d9a-a1bf-85289448ef1d" />

## 🎯 **Business Problem**
Manual data preparation on **70K+ bank loan records** took excessive time, hindering timely **risk analysis** and **profitability insights**.

## 💡 **Solution & Impact**
- **End-to-end ETL pipeline** designed using **PostgreSQL**
- **Automated SQL data cleaning & feature engineering** → **40% faster** process
- **Interactive Excel dashboards** with KPIs, pivot tables, slicers analyzing **default rates** and **profitability**
- Enabled **risk-based lending decisions** with improved visibility

## 🛠️ **Tech Stack**
- PostgreSQL (ETL Pipeline, Data Processing)
- Advanced SQL (Cleaning, Feature Engineering)
- Excel Advanced (Pivot Tables, Slicers, Dashboards)
- Financial Analytics (Risk, Profitability Metrics)


## 📊 **Key Features**

### **ETL Pipeline**
| Stage | SQL Operations | Impact |
|-------|----------------|--------|
| **Data Cleaning** | Remove duplicates, nulls, standardize formats | 40% faster prep |
| **Feature Engineering** | Risk scores, income-debt ratios, segment flags | Better predictions |
| **Analytics Tables** | Default rates, profitability by segment | Decision-ready |

### **Excel Dashboard Components**
- **KPIs**: Default Rate (8.2%), Profitability ROI, Risk Score
- **Pivot Tables**: Loan performance by region/customer segment
- **Slicers**: Filter by loan type, credit score, tenure
- **Charts**: Default trends, profitability heatmaps

## 🚀 **Quick Setup & Demo**
-- 1. Run ETL Pipeline

        psql -f sql_scripts/01_data_cleaning.sql
        
        psql -f sql_scripts/02_feature_engineering.sql

-- 2. Open Dashboard
        Loan_Analytics_Dashboard.xlsx → Refresh All → Explore slicers


## 📈 **Key Insights Generated**
- 💸 Default Rate: 8.2% (High-risk segments: 15%+)
- 📈 Top 20% customers generate 65% profitability
- ⚠️ Risk Reduction: 40% faster data prep → Better lending decisions
- 🎯 Actionable: Segment-wise risk thresholds identified


## 🎓 **Skills Demonstrated**
- ✅ PostgreSQL ETL Pipeline Design (End-to-End)
- ✅ Advanced SQL: Data Cleaning, Feature Engineering
- ✅ Excel Advanced Analytics: Pivot Tables, Slicers, Dynamic Dashboards
- ✅ Financial Risk Analysis: Default Rates, Profitability Metrics
- ✅ Process Automation: 40% Manual Effort Reduction
- ✅ Business Intelligence: Risk-Based Decision Support


## 📊 **Sample Data Preview**

**Raw Loans (70K+ rows)**
- loan_id,customer_id,loan_amount,interest_rate,default_flag
- L001,C001,500000,12.5,0
- L002,C002,750000,14.2,1

**Analytics Output**
-- Default rate by credit score bucket

    SELECT
    
    credit_score_bucket,
    
    COUNT(*) as total_loans,
    
    AVG(default_flag) as default_rate
    
    FROM clean_loans
    
    GROUP BY credit_score_bucket;

## 📈 **Resume Bullet Points**
- Designed PostgreSQL ETL pipeline processing 70K+ loan records → 40% faster data prep
- Automated SQL cleaning/feature engineering reducing manual effort by 40%
- Created Excel dashboards analyzing default rates/profitability enabling risk-based lending
