# Academic Data Warehouse Development for Decision Support

## Overview

This project focuses on the development of an **Academic Data Warehouse (DW)** designed to support decision-making processes within a university academic administration system.

The data warehouse integrates multiple academic datasets into a centralized analytical database using **dimensional modeling with a Star Schema structure**. Data is processed through a structured **ETL (Extract, Transform, Load) pipeline** to ensure data quality, consistency, and historical tracking before being used for analytical queries and reporting.

The system enables academic administrators and decision-makers to analyze student performance, monitor academic trends, and generate insights through interactive dashboards.

---

## Objectives

The objectives of this project include:

* Integrating academic datasets into a centralized data warehouse
* Implementing dimensional modeling using a **Star Schema**
* Developing ETL processes for data extraction, transformation, and loading
* Ensuring data quality through validation and integrity checks
* Supporting analytical queries and reporting for academic decision-making

---

## Data Warehouse Architecture

The system uses a **Star Schema architecture** consisting of one fact table and several dimension tables.

### Fact Table

**Fact_Enrollment**

Measures stored in this table include:

* Credits
* Grade
* GradePoint
* AttendanceRate
* TuitionFee
* Other academic performance indicators

### Dimension Tables

* Dim_Student
* Dim_ProgramStudy
* Dim_Status
* Dim_Gender
* Dim_Date

This structure enables efficient **multidimensional analysis** across student attributes, academic programs, status, and time periods.

---

## ETL Process

The ETL pipeline was implemented using **SQL Server Stored Procedures**.

### Extract

Data is extracted from academic datasets and loaded into **staging tables**.

### Transform

The transformation stage performs:

* Data cleaning
* Data normalization
* Handling missing values
* Removing duplicates
* Standardizing formats
* Applying **Slowly Changing Dimension (SCD Type 2)** for historical tracking

### Load

The cleaned and transformed data is loaded into **dimension tables and fact tables** in the data warehouse.

The ETL workflow is managed using the master procedure:

```
usp_Master_ETL
```

---

## Data Quality Assurance

To ensure data reliability, several validation processes were implemented:

* Data completeness checks
* Accuracy validation
* Referential integrity checks
* Duplicate detection
* Data reconciliation between staging and warehouse tables

These processes ensure consistent and reliable analytical data.

---

## Dashboard & Analytics

An interactive **Power BI dashboard** was developed to provide analytical insights, including:

* Student academic performance
* Average GPA trends
* Distribution of student academic status
* Identification of at-risk students
* Academic trends across different cohorts

The dashboard supports multiple analytical perspectives including **executive summaries, analytical exploration, and detailed academic monitoring**.

---

## Technologies Used

* SQL Server
* SQL Server Management Studio (SSMS)
* Power BI
* Dimensional Modeling (Star Schema)
* ETL using Stored Procedures
* Data Cleaning & Validation

---

## Key Outcomes

* Centralized academic data repository
* Improved academic reporting efficiency
* Historical tracking of academic data using SCD Type 2
* Optimized analytical queries through indexing and structured data modeling
* Interactive dashboards supporting academic decision-making

---

## Author

Keren Marito Lumban Gaol
Data Science Student – Institut Teknologi Sumatera (ITERA)

## Dashboard Preview

![Academic Dashboard](dashboard.png)
