# Atliq Hardwares: Financial & Sales Analytics

## Project Objective
This project transforms raw transactional data into a suite of dynamic, automated financial reports for Atliq Hardwares. The goal was to build a robust data model entirely within the Microsoft Excel ecosystem (Power Query & Power Pivot) to analyze customer behavior, market-vs-target performance, and Profit & Loss (P&L) metrics across multiple fiscal periods.

## Tech Stack & Tools Used
* **Microsoft Excel:** Pivot Tables, Advanced Conditional Formatting, XLOOKUP, INDEX MATCH.
* **Power Query:** ETL processes, Data Cleaning, Custom M Query Code.
* **Power Pivot:** Data Modeling (Star Schema), Diagram View.
* **DAX (Data Analysis Expressions):** Custom measures for financial metrics.

## Methodology & Workflow

### 1. Data Extraction & Cleaning (Power Query)
* Extracted raw data from multiple sources into Power Query.
* Performed essential ETL (Extract, Transform, Load) steps: standardizing data types, handling missing values, and filtering anomalies.
* Created a dynamic, dedicated **Date Table using custom M query code** to enable accurate time-intelligence calculations across fiscal years and quarters.

### 2. Data Modeling (Power Pivot)
* Loaded the cleaned datasets directly into the Power Pivot Data Model to bypass Excel's row limits.
* Constructed a **Star Schema** in the Diagram View, establishing one-to-many relationships between Dimension tables (Customers, Markets, Products, Date) and Fact tables (Sales, Targets).
* Mapped Primary Keys to Foreign Keys to ensure seamless cross-filtering across all reports.

### 3. DAX Calculations & Advanced Functions
* Wrote custom DAX measures for core KPIs: `Net Sales`, `COGS` (Cost of Goods Sold), `Gross Margin`, and `GM %`.
* Utilized `XLOOKUP` and `INDEX MATCH` for auxiliary data retrieval and validation outside the core pivot tables.
* Calculated dynamic year-over-year (YoY) growth and target variance metrics.

### 4. Reporting & Visualization
Developed five interconnected reports using Excel Pivot Tables:
1. **Customer Performance Report:** Analyzes Net Sales performance across key clients with YoY comparison.
2. **Market Performance vs Target Report:** Tracks regional sales against predefined targets, highlighting deficits.
3. **P&L Statement by Fiscal Year:** High-level summary of financial health over three years.
4. **P&L Statement by Markets:** Granular breakdown of COGS and Gross Margin percentages by country.
5. **P&L Statement by Months:** Detailed quarterly and monthly trending of Net Sales and Margins.
* Applied extensive **Conditional Formatting** (data bars, color scales, and custom font colors) to instantly highlight negative variances and top performers.

## Repository Assets
* `Atliq_Financial_Analytics.xlsx`: The core workbook containing the data model and reports.
* `/assets`: Folder containing high-resolution 4:5 screenshots of the final reports.
