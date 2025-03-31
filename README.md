# Report Generation using Databricks

Report Generation using Databricks
 
Overview
 
This project generates reports on daily, weekly, and monthly basis using sales data available in CSV files. The reports are generated using a Databricks notebook, which provides an option to select the report frequency using a dropdown menu.
 
Requirements
 
- Databricks account with access to a cluster
- Sales data in CSV files
- Databricks notebook with necessary libraries and dependencies
 
Agenda
 
1. *Data Ingestion*: Load sales data from CSV files into a Databricks dataframe.
2. *Report Generation*: Create a Databricks notebook with a dropdown menu to select the report frequency (daily, weekly, monthly).
3. *Query Execution*: Automatically execute the relevant query based on the selected report frequency.
4. *Report Display*: Display the generated report in a readable format.
 
Notebook Structure
 
The Databricks notebook will consist of the following sections:
 
1. *Import Libraries*: Import necessary libraries and dependencies.
2. *Load Data*: Load sales data from CSV files into a Databricks dataframe.
3. *Report Frequency Selection*: Create a dropdown menu to select the report frequency.
4. *Query Execution*: Execute the relevant query based on the selected report frequency.
5. *Report Display*: Display the generated report in a readable format.
 
Queries
 
The following queries will be used to generate the reports:
 
- *Daily Report*: `SELECT * FROM sales_data WHERE date = yesterday()`
- *Weekly Report*: `SELECT * FROM sales_data WHERE date >= date_trunc('week', current_date) - interval '1 week'`
- *Monthly Report*: `SELECT * FROM sales_data WHERE date >= date_trunc('month', current_date) - interval '1 month'`
 
Report Format
 
The reports will be displayed in a readable format, including:
 
- *Date*: Date of the sales data
- *Sales*: Total sales amount
- *City*: City where the sales were made
 
Usage
 
1. Open the Databricks notebook and select the report frequency using the dropdown menu.
2. Execute the notebook to generate the report.
3. View the generated report in a readable format.
