# Data Warehouse and Analytics Project
 
Welcome to my **Data Warehouse and Analytics Project** repository! 🚀  
This project demonstrates an end-to-end data warehousing and analytics solution, from ingesting raw source files to generating actionable business insights with SQL. Built as a portfolio project, it follows industry best practices in data engineering and analytics.
 
---
 
## 🏗️ Data Architecture
 
The warehouse follows the **Medallion Architecture** with **Bronze**, **Silver**, and **Gold** layers:
 
1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV files into a SQL Server database.
2. **Silver Layer**: Handles data cleansing, standardization, and normalization to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema for reporting and analytics.
```
 CSV Files (ERP + CRM)
        │
        ▼
 ┌─────────────┐     ┌──────────────┐     ┌──────────────┐
 │   BRONZE    │ ──▶ │    SILVER    │ ──▶ │     GOLD     │
 │  Raw data   │     │ Cleaned data │     │ Star schema  │
 └─────────────┘     └──────────────┘     └──────────────┘
                                                  │
                                                  ▼
                                       Analytics & Reporting
```
 
---
 
## 📖 Project Overview
 
This project covers:
 
1. **Data Architecture**: Designing a modern data warehouse using Medallion Architecture (Bronze, Silver, Gold).
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Building fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Writing SQL-based reports to surface business insights.
🎯 Skills demonstrated:
 
- SQL Development
- Data Engineering
- ETL Pipeline Development
- Data Modeling
- Data Analytics
---
 
## 🚀 Project Requirements
 
### Building the Data Warehouse (Data Engineering)
 
#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data and enable analytical reporting and informed decision-making.
 
#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues before analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization is not required.
- **Documentation**: Provide clear documentation of the data model for business stakeholders and analytics teams.
---
 
### BI: Analytics & Reporting (Data Analysis)
 
#### Objective
Develop SQL-based analytics to deliver detailed insights into:
 
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**
These insights give stakeholders key business metrics to support strategic decisions.
 
---
 
## 📂 Repository Structure
 
```
sql-datawarehouse-project/
│
├── dataset/          # Raw source datasets (ERP and CRM CSV files)
│
├── scripts/          # SQL scripts for ETL and transformations
│   ├── bronze/       # Extract and load raw data
│   ├── silver/       # Clean and transform data
│   ├── gold/         # Create analytical models (star schema)
│
├── tests/            # Data quality checks and test scripts
│
├── LICENSE           # MIT License
└── README.md         # Project overview and instructions
```
 
---
 
## ⚙️ Getting Started
 
**Prerequisites**
- SQL Server (Express or Developer edition)
- SQL Server Management Studio (SSMS) or Azure Data Studio
**Steps**
1. Clone the repository:
```bash
   git clone https://github.com/Prashast-Srivastava/sql-datawarehouse-project.git
```
2. Create the database and schemas (`bronze`, `silver`, `gold`).
3. Run the scripts in `scripts/bronze/` to create tables and load the CSV files from `dataset/`.
4. Run the scripts in `scripts/silver/` to clean and standardize the data.
5. Run the scripts in `scripts/gold/` to build the star schema views.
6. Run the checks in `tests/` to validate data quality.
---
 
## 🛡️ License
 
This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share this project with proper attribution.
 
---
 
## 🌟 About Me
 
Hi, I'm **Prashast Srivastava** 👋
 
I'm a final-year B.Tech Computer Science (Data Science) student at **BBDITM, Lucknow**, graduating in 2027. I'm building toward a career in **data engineering and data analytics**, with hands-on experience in Python, SQL, and machine learning.
 
I'm currently looking for **Data Analytics and Data Engineering internship** opportunities.
 
📫 **Let's connect**
 
- GitHub: [Prashast-Srivastava](https://github.com/Prashast-Srivastava)
- LinkedIn: [prashast-srivastava](https://www.linkedin.com/in/prashast-srivastava-)
- Email: prashastsrivstava@gmail.com
