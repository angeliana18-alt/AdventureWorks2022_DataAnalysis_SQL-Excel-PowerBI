# Adventure Works Cycle
A Microsoft Power BI business intelligence dashboard for Adventure Works Cycle — sales performance, quality control, and supply chain reporting for the Adventure Works cycling-equipment manufacturing dataset.

The report connects directly to a SQL Server instance via three purpose-built views — `SalesPerformanceFacts`, `QualityControlFacts`, `SupplyChainFacts` — each pre-joined and pre-aggregated at the source rather than modeled as a relational star schema inside Power BI. Fiscal periods run July–June (not calendar year); Fiscal Year 2011 is a partial year, starting in May. Territory reporting is normalized to 6 named regions, with the 5 U.S. sales territories merged into a single `US` value.

<img alt="AdventureWorks2022_DataAnalysis_SQL-Excel-PowerBI" src="Screenshots/SalesPerformance Dashboard.gif">

## Features

- Track headline KPIs — revenue, profit, profit margin, and units sold.
- Compare sales across product category and sales territory.
- Analyze monthly trend patterns for every KPI
- Monitor manufacturing quality — scrap cost, scrap-cost ratio, defect rate, production cost.
- Track supply chain performance.

## Project Highlights

This project involved the following tasks:

- connecting and transforming raw data
- building project panel tables
- building individual KPI queries using advanced SQL functions
- creating calculated columns and measures using DAX
- creating **dynamic label measures**
- building an interactive dashboard

## Dashboard Elements

#### Sales Performance

- High-Level KPIs for Revenue, Profit, Profit Margin Sold Products
- Page-level filtering by Product Category,Territory and Fiscal Year
- Drill-Through Monthly Revenue, Profit, Top 5 Product SubCategory Revenue and Top 5 Product Sub Category Average Discount

#### Quality Control

- **Production Cost** and **Scrap Cost analysis**

#### Supply Chain

- **Avg Lead Time** — analysis

### Insights

- Approximately $ 109.9 million in revenue and $ 12.5 million in profit was generated between 31-05-2011 and 30-06-2014.
    - There are several appreciable dips in profit, possibly due to heavy discounting:
        - Fiscal year 2012 April: profit actually goes negative, approximately -$350 thousand;
        - Fiscal year 2013  May-June: although revenue is at its highest in June approximately $5 million, while profit is at its lowest approximately for may at $50 thousand and June at $100 thousand
        - Fiscal year 2014 July with profit at approximately at $75 thousand
    - **Fiscal Year 2014** is approximately **$6.2 million** of the **$ 12.5 million all time profit — 49.7%.**
    With a converted revenue to profit at a noticeably better rate than the other three years combined.
    
    Making it an exceptional year, and it would be worth investigated the cause of this.
    Was this due to simply the larger crashes in the previous years of a young growing company and 2014 as the beginning of a mature company? 
    
- While US has the largest market with $ 63 miliion in total revenue, The Australian market has the largest revenue to profit conversion rate with 33.5% in total profit margin.
    
<img alt="AdventureWorks2022_DataAnalysis_SQL-Excel-PowerBI" src="Screenshots/Revenue vs ProfitMargin - Market US.png">
    
<img alt="AdventureWorks2022_DataAnalysis_SQL-Excel-PowerBI" src="Screenshots/Revenue vs ProfitMargin - Market Australia.png">
    
- Fiscal year 2014 is the most scrap-efficient full year on record, despite being the highest-volume year.

<img alt="AdventureWorks2022_DataAnalysis_SQL-Excel-PowerBI" src="Screenshots/QualityControl Dashboard.gif">

##
