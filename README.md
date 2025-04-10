# SQL---DataWarehouse
<p>Welcome to SQL---DataWarehouse Project repository!</p>
<p>This project includes comprehensive data warehousing and analytics solutions commonly used in the industry.</p>
<p>It was designed as a portfolio project.</p>

Inspired by [DataWithBaraa](https://www.youtube.com/@DataWithBaraa).

## 📋 Table of Contents
 - <strong>Project Overview</strong>
 - <strong>Data Architecture</strong>
 - <strong>Project Requirements</strong>
 - <strong>Repository Structure</strong>
 - <strong>Tools used in the Project</strong>
 - <strong>About me</strong>

## 🔍 Project Overview
<p>This project is divided into two parts.</p>
<p>First part showcases the process of building data warehouse, covering full road from raw CSV data files up to developing structured fact and dimension tables optimized for analytical queries.</p>

 - <strong>Data Architecture</strong>: This data warehouse uses Medallion Architecture, containing three (Bronze, Silver, Gold) layers.
 - <strong>ETL process</strong>: Extracting, transforming and loading data from source into consecutive warehouse layers.
 - <strong>Data Modeling</strong>: Developing prepared for data analysis fact and dimension tables.

Second part demonstrates advanced techniques frequently used by professional data analytics and brings up final reports about customers and products in the business.
 - <strong>Analytics & Reporting</strong>: Creating SQL-based reports for actionable insights.

## 🏛️ Data Architecture
<p>Project follows <strong>Medallion Architecture</strong> with <strong>Bronze</strong>, <strong>Silver</strong> and <strong>Gold</strong> layers: </p>

![Data Architecture](data_warehouse/docs/data_architecture.png)

 - <strong>Bronze Layer</strong>: Stores raw data, as-is from source systems. Data is loaded from CSV files into the SQL Server Database with stored procedure. No transformations are performed.
 - <strong>Silver Layer</strong>: This layer includes data cleansing, standarization and normalization processes in order to prepare data for analysis. Data is loaded from Bronze layer into Silver layer with stored procedure. 
 - <strong>Gold Layer</strong>: Contains business-ready data modeled into star schema prepared for analysis. Data is stored in views.
 
## 📌 Project Requirements
### Building the Data Warehouse (Data Engineering)
<strong>Objective</strong>: Develop a modern data warehouse using SQL Server to consolidate data and prepare it for analytical reporting and infromed decision-making.

<strong>Specifications</strong>:
 - <strong>Data Sources</strong>: Import data from two source systems (CRM and ERP) provided as CSV files.
 - <strong>Data Quality</strong>: Cleanse and normalize data resolving its quality issues prior to analysis.
 - <strong>Integration</strong>: Combine both sources into single, user-friendly data model designed for analytical reporting.
 - <strong>Scope</strong>: Focus on the latest dataset only, historization is not required.
 - <strong>Documentation</strong>: Provide clear documentation of the data model to support further users of data warehouse.

### BI: Analytics & Reporting (Data Analysis)
<strong>Objective</strong>: Develop SQL-based analytics to deliver detailed insights about the business.
 - <strong>Customer Behaviour</strong>
 - <strong>Product Performance</strong>
 - <strong>Sales Trends</strong>
 
These insights empower stakeholders with key business metrics.

## 🗂️ Repository Structure
```
SQL---DataWarehouse/

data_warehouse/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details
│   ├── data_integration.drawio         # Draw.io file shows how the tables are related
│   ├── data_architecture.drawio        # Draw.io file shows the project's architecture
│   ├── data_architecture.png           # PNG file shows the project's architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow_diagram.drawio        # Draw.io file for the data flow diagram
│   ├── sales_data_mart.drawio          # Draw.io file for data models (star schema)
│   ├── naming-conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│   ├── init_database.sql               # Script for initialization of database
│
├── tests/                              # Test scripts and quality files

data_analysis/
│
├── docs/                               # Project documentation and analysis details
│   ├── data_analysis_roadmap.drawio    # Draw.io file shows particular steps of analysis
│
├── scripts/                            # SQL scripts for data analysis
│   ├── ada_change_over_time.sql        # SQL script for change-over-time analysis
│   ├── ada_cumulative_analysis.sql     # SQL script for cumulative analysis
│   ├── ada_data_segmentation.sql       # SQL script for data segmentation
│   ├── ada_part_to_whole_analysis.sql  # SQL script for part-to-whole analysis
│   ├── ada_performance_analysis.sql    # SQL script for performance analysis
│   ├── eda_database_exploration.sql    # SQL script for database exploration
│   ├── eda_date_exploration.sql        # SQL script for date exploration
│   ├── eda_dimensions_exploration.sql  # SQL script for dimensions exploration
│   ├── eda_magnitude_analysis.sql      # SQL script for magnitude analysis
│   ├── eda_measures_exploration.sql    # SQL script for measures exploration
│   ├── eda_ranking_analysis.sql        # SQL script for ranking analysis
│   ├── customers_report.sql            # SQL file for final customers report
│   ├── products_report.sql             # SQL file for final products report

README.md                               # Project overview and instructions

```
---

## ⚒️ Tools used in the Project
 - [SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) - Lightweight server for hosting SQL database.
 - [SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16) - GUI for managing and interacting with database.
 - [Draw.io](https://www.drawio.com/) - Design data architecture, dataflows, models and diagrams.
 - [Notion](https://www.notion.com/) - For project management and organization.
 - [GitHub](https://github.com/) - Repository to manage version and collaborate on the code.

## 🙋 About me
My name is Mateusz Dąbrowski, and I hold a Bachelor's degree in Telecommunications and Computer Science. Below you can find the links to my profiles, feel free to browse or contact me!

[![LinkedIn](https://img.icons8.com/?size=100&id=xuvGCOXi8Wyg&format=png&color=000000)](https://www.linkedin.com/in/mateusz-d%C4%85browski-7634b0205/) [![Tableau](https://img.icons8.com/?size=100&id=9Kvi1p1F0tUo&format=png&color=000000)](https://public.tableau.com/app/profile/mateusz.d.browski3656/vizzes)

