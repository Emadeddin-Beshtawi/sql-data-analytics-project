# SQL Data Analytics Project

## Introduction  

This project demonstrates advanced **SQL Analytics** on top of a Medallion-style Data Warehouse (Bronze, Silver, Gold) implemented in SQL Server. It builds on the cleaned and structured Gold Layer to deliver actionable insights through trend analysis, performance benchmarking, segmentation, and business reporting.


---
## Scenario / Problem Statement  
Organizations need to move beyond raw data and exploratory analysis to **business-ready analytics**.  
This project answers real business questions such as:  
- How do key metrics change over time?  
- What are the cumulative growth patterns?  
- Which products and customers are high performers?  
- How do different segments contribute to overall results?  
- What KPIs can guide decisions at the executive level?  
---
## Objectives  
- Apply SQL-based analytics over a curated Gold Layer.  
- Deliver **repeatable, parameter-free scripts** for time-series, cumulative, segmentation, and benchmarking analysis.  
- Provide **customer and product reports** as views for direct consumption.  
- Showcase SQL analytical functions such as **LAG, SUM OVER, CASE, DATEPART** for real-world use cases.  
---
## Datasets Used
The underlying datasets are provided by the vendored **Data Warehouse**:

**CRM (source_crm/)**
- `cust_info.csv` — customer master
- `prd_info.csv` — product master
- `sales_details.csv` — sales order lines

**ERP (source_erp/)**
- `CUST_AZ12.csv` — customer demographics
- `LOC_A101.csv` — customer country
- `PX_CAT_G1V2.csv` — product category metadata

> These are available in this repo via `https://github.com/Emadeddin-Beshtawi/sql-data-warehouse-project`
---
## Repository Structure  
```text
sql-data-analytics-project/
├── scripts/
│ ├── 01_change_over_time_analysis.sql
│ ├── 02_cumulative_analysis.sql
│ ├── 03_performance_analysis.sql
│ ├── 04_data_segmentation.sql
│ ├── 05_part_to_whole_analysis.sql
│ ├── 06_report_customers.sql
│ └── 07_report_products.sql
├── deps/
│ └── data-warehouse/ # vendored DW repo (tag v1.0.1)
├── README.md
├── LICENSE
└── .gitignore
```

---
## Conclusion  
- This project showcases **SQL Analytics skills** by implementing trend analysis, segmentation, benchmarking, and consolidated reports on a Medallion DW.  
- It highlights the ability to move from structured, ETL-prepared data to **business insights**, an essential step in real-world analytics pipelines.  

---
## Related Projects  
- [SQL Data Warehouse Project](https://github.com/Emadeddin-Beshtawi/sql-data-warehouse-project)  
- [SQL Exploratory Data Analysis (EDA) Project](https://github.com/Emadeddin-Beshtawi/sql-exploratory-data-analysis-project)  
