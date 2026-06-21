# Sales Analysis: Full-Stack Data Engineering & Analytics Pipeline

An end-to-end data pipeline transforming 3,900 e-commerce records. This project covers the entire engineering lifecycle: local categorical imputation and feature engineering in Python, automated ETL orchestration via SQLAlchemy to a production PostgreSQL database, complex server-side analytical window functions, and an interactive Power BI executive dashboard.

##  Architecture & Tech Stack
*   **Data Wrangling & ETL:** Python 3, Pandas, NumPy, SQLAlchemy
*   **Database Management:** PostgreSQL
*   **Business Intelligence:** Power BI Desktop

---

##  Engineering Lifecycle & Implementation

### 1. Data Wrangling & Feature Engineering (Python)
*   **Profile Analysis:** Evaluated a raw retail dataset consisting of 3,900 customer records across 18 features (~548.6 KB).
*   **Data Cleaning:** Implemented localized categorical median imputation to accurately handle missing values in `Review Rating` without introducing statistical bias.
*   **Feature Engineering:** Utilized `pd.qcut()` to perform generational age-group binning, segmenting customer demographics for downstream analysis.

### 2. Database Orchestration & Analytics (PostgreSQL)
*   **Automated Migration:** Built an automated ETL script using SQLAlchemy to seamlessly ingest cleaned Python DataFrames into a production PostgreSQL instance.
*   **Advanced SQL Modeling:** Authored 10 complex analytical queries utilizing Common Table Expressions (CTEs) and `ROW_NUMBER()` window functions to:
    *   Segment customers dynamically into *New*, *Returning*, and *Loyal* cohorts.
    *   Rank and optimize category-specific inventory.

### 3. Executive Visualization (Power BI)
*   **Dashboard Architecture:** Designed an interactive, 4-quadrant executive dashboard adhering to UI/UX best practices.
*   **Layer Optimization:** Resolved visual clipping and formatting bugs by structuring element depth using the Power BI Selection Pane.
*   **Interactivity:** Enabled seamless cross-filtering across customer demographics, product categories, and logistics channels.

---

## 📊 Core Business Findings & Insights

*   **The Loyalty Paradox:** Analysis revealed that subscription status does not significantly impact purchasing volume; subscribers and non-subscribers maintain highly similar average order spends.
*   **Revenue Anchor:** The **Clothing** department stands as the primary revenue driver, contributing **$104K** to total sales.
*   **Logistics Correlate:** Customers selecting **2-Day Shipping** exhibited the highest Average Order Value (**$60.73**), surfacing a major high-value logistics optimization opportunity.

---
