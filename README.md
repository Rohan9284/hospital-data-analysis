# hospital-data-analysis

Healthcare Operations & Financial Analysis Pipeline
An end-to-end data project transforming raw, messy healthcare records into a high-impact executive dashboard. This project demonstrates a full ETL (Extract, Transform, Load) pipeline using Python and SQL, finishing with an interactive Power BI report to optimize hospital billing and insurance provider relationships.

🎯 Problem Statement
Hospital administrators often struggle with "dirty" synthetic data and fragmented billing records. The goal of this project was to:

Clean & Validate 55,000+ patient records (handling negative billing errors and inconsistent naming).

Analyze Revenue to identify which medical conditions (e.g., Obesity, Diabetes) generate the highest costs.

Optimize Insurance Relations by identifying which providers cover the most expensive treatments.

🛠️ Tech Stack
Language: Python (Pandas, Numpy) for Data Cleaning.

Database: SQL (SQLite) for Relational Data Modeling & Querying.

Visualization: Power BI for Interactive Dashboards.

Environment: Google Colab for the development environment.

🚀 The Pipeline (Step-by-Step)
1. Data Engineering (Python)
Extraction: Loaded the raw healthcare_dataset.csv.

Transformation: * Standardized names to Title Case.

Converted date strings into DateTime objects.

Data Quality Fix: Identified and removed 108 records with negative billing amounts (data entry errors).

Feature Engineering: Created length_of_stay and a unique admission_id.

2. Database Management (SQL)
Loaded the "Gold Standard" data into a SQLite database.

Performed complex aggregations to calculate total revenue per insurance provider and condition.

Key Query: Identified Blue Cross and Obesity as the #1 revenue-generating segment ($49.3M).

3. Business Intelligence (Power BI)
Built an interactive dashboard featuring:

Executive KPIs: Total Revenue, Unique Patient Count, and Avg Hospital Stay.

Financial Breakdown: Stacked bar charts showing costs by Medical Condition.

Interactive Slicers: Filter by Admission Type (Urgent vs. Elective) and Test Results.

📊 Key Insights
Top Condition: Obesity is the most expensive condition treated, followed closely by Diabetes.

Insurance Performance: Blue Cross and Medicare account for the highest volume of high-billing patients.

Operational Efficiency: 33% of admissions are marked as "Urgent," requiring higher resource allocation.

📂 Project Structure
Plaintext
├── data/
│   ├── raw_healthcare_data.csv        # Original Kaggle Data
│   └── gold_standard_healthcare.csv   # Cleaned Data (Ready for BI)
├── notebooks/
│   └── healthcare_pipeline.ipynb      # Full Python/SQL Cleaning Code
├── dashboard/
│   └── Healthcare_Analytics.pbix      # Power BI Dashboard File
└── README.md
💡 How to Run
Clone this repository.

Open the healthcare_pipeline.ipynb in Google Colab or Jupyter to see the cleaning process.

Download the gold_standard_healthcare.csv.

Open the Power BI file and refresh the data source to see the visuals.

Author
[Your Name]
