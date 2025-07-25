# Atliq-Hardware-Problem-Statement---In-Excel
Excel - Atliq Hardware Problem Statement
Agenda:
This project focuses on Sales and Financial Analysis for Atliq Hardware, implementing a structured ETL (Extract, Transform, Load) process.

Extract: Received 4 primary tables:

dim_customer

dim_market

dim_product

fact_sales_monthly

Sales Report
Project Objectives:
Customer Performance Report – https://github.com/bb1608/Atliq-Hardware-Problem-Statement---In-Excel/blob/main/Customer%20Performance%20Report.pdf

Market Performance vs. Sales Targets – https://github.com/bb1608/Atliq-Hardware-Problem-Statement---In-Excel/blob/main/Markel%20Performance%20vs%20Target%20report.pdf

Purpose of Sales Analytics:
Enable businesses to monitor and evaluate sales performance across customers and markets.

Importance of Analyzing Sales Data:
Identify sales patterns and KPIs to drive strategic decisions.

Determine effective customer discounts and explore market expansion opportunities.

Key Learnings & Implementation:
Followed Report Solution Design Process to map report components to respective tables:

Net Sales – from fact_sales_monthly

Year – derived using a new dim_date table via Power Query (learned functions like Date.AddMonths, Date.Year)

Division – from dim_product

Country & Region – from dim_market

Customer – from dim_customer

Used Power Query Reference to manage multiple datasets during extraction.

Created DAX measures (e.g., CALCULATE) to resolve pivot table layout issues and compute KPIs like 21 vs 20 Net Sales.

Built filters by market, region, and division for deep dive analysis.

Market Performance vs Targets Report
Combined historical sales data (2019–2021) with country-wise monthly targets from ns_targets_2021.

Key step: Mapped "Market" to "Country" to align targets with performance.

Finance Report
Project Objectives:
Profit & Loss (P&L) Reports by Fiscal Year – https://github.com/bb1608/Atliq-Hardware-Problem-Statement---In-Excel/blob/main/Profit%20%26%20Loss%20Statement%20by%20Fiscal%20Year.pdf

P&L Report & Months 

P&L Reports by Markets – [View Report.](https://github.com/bb1608/Atliq-Hardware-Problem-Statement---In-Excel/blob/main/Profit%20%26%20Loss%20Statement%20by%20Market.pdf)

Purpose of Financial Analytics:
Evaluate profitability, assist in budgeting/forecasting, and communicate performance to stakeholders.

Key Learnings & Implementation:
Integrated new financial datasets (renamed as Finance Reference) and updated the data model.

Created COGS, Gross Margin, GM% using calculated columns:

Total_COGS = Freight_Cost + Manufacturing_Cost.

Built P&L metrics by months & quarters.

Applied functions like IFERROR to handle missing values and improve report reliability.

Gained knowledge on fiscal years and months in financial reporting.

Technical & Soft Skills
Technical Skills:
Proficiency in ETL methodology (Extract, Transform, Load).

Creating date tables in Power Query.

Deriving fiscal months and quarters.

Building data model relationships with Power Pivot.

Using DAX measures (e.g., CALCULATE, IFERROR) and calculated columns.

Integrating supplementary datasets into an existing model.

Soft Skills:
In-depth understanding of Sales & Finance reports.

Designing user-centric reports with a focus on clarity and decision-making.

Optimizing report generation through systematic fine-tuning.

Developing a structured report-building plan following Report Solution Design Process.

Key Takeaways from the Project
Learned how to map components to specific tables for effective report building.

Acquired hands-on experience with Power Query Reference, dim_date creation, and date functions.

Developed Market Performance vs Targets and P&L reports using advanced Power Pivot and DAX.

Enhanced ability to transform raw sales and financial data into strategic business insights.
