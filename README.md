# 🏥 Healthcare Operations & Financial Analysis Pipeline
> **End-to-End Data Engineering & Analytics Project**

---

## 📌 Executive Summary
This project addresses the challenge of managing and analyzing large-scale healthcare datasets. I built a robust **ETL pipeline** to clean 55,000+ patient records, uncovering critical insights into hospital revenue and insurance efficiency.

**Key Achievement:** Identified that **Obesity** treatments under **Blue Cross** insurance represent the highest revenue segment ($49.3M).

---

## 🛠️ Tech Stack
* **Data Engineering:** Python (Pandas)
* **Data Storage:** SQL (SQLite)
* **Analytics:** Power BI (DAX, Interactive Dashboards)

---

## 🚀 Project Workflow

### 1. Data Engineering (Python)
Using Python in [Google Colab](https://colab.research.google.com/drive/1r9MAbn57BCB0wfsVpYiiM6MrCij3RDSB), I transformed raw data into a "Gold Standard" dataset:
* **Quality Control:** Removed 108 records with negative/zero billing.
* **Standardization:** Converted names (e.g., "bObBy jAcKsOn") to Proper Title Case.
* **Feature Engineering:** Calculated `length_of_stay` and created a unique `admission_id`.

### 2. SQL Analysis
Migrated data to a SQL environment for deep-dive querying:
* **Revenue Mapping:** Ranked medical conditions by total billing.
* **Insurance Audit:** Analyzed provider volume vs. total payout.

### 3. Business Intelligence (Power BI)
Created an interactive dashboard for hospital managers:
* **KPI Cards:** Real-time tracking of Revenue and Patient counts.
* **Slicers:** Ability to filter the entire report by "Urgent" vs "Elective" admissions.

---

## 📊 Key Business Insights
* **High-Cost Drivers:** Obesity and Diabetes are the top revenue contributors.
* **Operational Strain:** 33% of all admissions are "Urgent," indicating high ER resource needs.

---

## 📂 Repository Structure
* `data/`: Raw and Cleaned CSV files.
* `python/`: [Google Colab Notebook](https://colab.research.google.com/drive/1r9MAbn57BCB0wfsVpYiiM6MrCij3RDSB) for ETL.
* `powerbi/`: `.pbix` Dashboard file.

---

### 👨‍💻 Developed by
Rohan Jadhav
