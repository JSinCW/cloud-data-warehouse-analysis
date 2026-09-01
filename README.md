# Cloud Data Warehouse Analysis

## Project Overview

This project explores cloud-based data warehousing and SQL analysis using **AWS Redshift Serverless** and **Google BigQuery**.

The work focuses on comparing query execution plans, understanding query cost, working with public cloud datasets, and using SQL to filter, aggregate, and analyze large datasets.

## Tools Used

- AWS Redshift Serverless
- Google BigQuery
- SQL
- BigQuery CLI (`bq`)
- Public cloud datasets

## AWS Redshift Analysis

Two SQL queries were compared using the Redshift sample `tickitdb` database.

Both queries returned the same result:

**Sum of quantity sold = 46**

However, the second query applied an additional date filter to the sales table before the join, which reduced the amount of data processed and resulted in a lower estimated query cost.

This demonstrated how filtering earlier in a query can improve efficiency.

## Google BigQuery Analysis

The BigQuery portion used public datasets including:

- GDELT
- BigQuery Natality dataset

Tasks included:

- Running SQL queries on public cloud datasets
- Filtering large datasets
- Using subqueries
- Aggregating results with `COUNT` and `GROUP BY`
- Ordering and limiting query results
- Reviewing estimated data processed and execution cost
- Inspecting table schemas using `bq show`
- Running queries using `bq query`

## Key Takeaways

- Query structure can affect processing cost even when results are identical.
- Applying filters earlier can reduce the amount of data scanned.
- Cloud data warehouses allow SQL-based analysis of large public datasets.
- Query-cost awareness is important when working with large-scale cloud platforms.

## Project Type

Academic Cloud Data Warehousing Assignment — California State University, East Bay

## Project File

- [View Cloud Data Warehouse Analysis](Cloud_Data_Warehouse_Analysis.pdf)
