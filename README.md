# RetailEdge Canada — Power BI Analytics

![Dashboard Preview]("Executive_Summary.png")

## Project Overview
End-to-end Power BI analytics solution for a national retail chain 
operating 10 stores across Canada. Built entirely from a single 
50,000-row raw CSV file using Power Query, Star Schema modelling, 
and DAX.

## Dataset
- 50,000 sales transactions (2022–2024)
- 10 stores across 6 Canadian provinces
- 800 products across 8 categories
- 150 employees
- 72,000 inventory snapshots

## What I Built

### Data Model
- Extracted 6 tables from 1 raw CSV using Power Query M code
- Star Schema with 2 fact tables (Sales + Inventory)
- 10 relationships with conformed dimensions
- Integer surrogate keys on all dimensions
- Custom Dim_Date table with time intelligence support

### DAX Measures (12 total)
- Total Revenue, Gross Profit, Units Sold, Transactions
- Gross Margin %, Return Rate %, Avg Order Value
- Online Revenue (CALCULATE)
- Revenue Last Year (SAMEPERIODLASTYEAR)
- YoY Revenue Growth %
- Critical Stock Items (cross-fact)
- Revenue % of Total (ALL)

### Dashboard (3 pages)
**Page 1 — Executive Summary**
![Executive Summary](page1-executive-summary.png)

**Page 2 — Store Performance**
![Store Performance](page2-store-performance.png)

**Page 3 — Inventory Health**
![Inventory Health](page3-inventory-health.png)

## Key Insights
- Electronics is the top revenue category (~2x nearest competitor)
- Toronto Downtown and Montreal Centre lead store revenue
- In-Store channel = 55% of revenue, Online growing at 35%
- 3,646 critical stock situations identified across all stores
- Automotive category has highest critical inventory risk

## Tools Used
- Power BI Desktop
- Power Query (M code)
- DAX
- Star Schema / Dimensional Modelling

## Skills Demonstrated
- ETL pipeline from raw flat file to dimensional model
- Surrogate key implementation
- Many-to-one relationship configuration
- Time intelligence DAX functions
- Cross-fact table analysis
- Executive dashboard design
