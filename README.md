# Predictive Customer Churn Control Tower

## Project Overview
This project is an end-to-end data analytics and machine learning pipeline designed to identify at-risk customers before they leave a service (churn). By generating and processing a synthetic dataset of 5,000 customers, this project demonstrates the ability to execute full-stack data engineering, predictive modeling, and executive-level visualization.

## Tech Stack & Tools
* **Data Engineering & ETL:** Python (Pandas, NumPy)
* **Machine Learning:** Scikit-Learn (Random Forest Classifier)
* **Data Visualization:** Power BI (DAX, Power Query)
* **Environment:** Jupyter Notebook, VS Code

## Project Architecture & Flowchart
The project follows a strict chronological data pipeline:

[Raw Data Generation] 
       │
       ▼
[ETL Pipeline] ➔ (Handle Missing Values, Remove Outliers, Feature Engineering)
       │
       ▼
[Machine Learning] ➔ (Train Random Forest Model ➔ Assign Churn Probability Score)
       │
       ▼
[Power BI Dashboard] ➔ (DAX Measures, Interactive Slicers, Action Matrix)

## Key Business Insights
1. **Revenue at Risk:** Accurately quantified the exact monthly recurring revenue tied to high-risk customers, allowing targeted financial interventions.
2. **Support Ticket Thresholds:** Identified a critical threshold where customers logging more than 7 support tickets show an exponential spike in churn probability.
3. **Actionable Slicing:** Built a dynamic matrix filtering only customers with a >70% churn risk, giving retention teams an immediate "call list" of high-risk accounts.

## Repository Structure
* `/data/raw/` - The initial synthetic datasets containing intentional anomalies.
* `/data/processed/` - Cleaned data post-ETL processing.
* `/data/final/` - The final output from the ML model containing the generated `ChurnRiskScore_%`.
* `data_pipeline.ipynb` - The complete Python codebase for data generation, ETL, and Machine Learning.
* `churn_dashboard.pbix` - The functional Power BI dashboard file.
* `dashboard_screenshot.pdf` - A high-resolution export of the final executive dashboard.

## 👨‍💻 Author
**Tanay Singh** 
*B.Sc. (Hons) Biotechnology, Amity University Lucknow*
