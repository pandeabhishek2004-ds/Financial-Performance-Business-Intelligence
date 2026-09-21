Financial Performance & Business Intelligence
A Power BI portfolio project focused on understanding financial performance, profitability, discount exposure and business risk from a management point of view.

Why I built this
I did not want to make another dashboard that only shows Sales, Profit and Products.

I wanted to answer a few practical business questions:

Where is the business making money?
Which segments and countries are contributing more profit?
Which products are creating losses?
How much discount exposure is there?
Where is profitability under pressure?
What areas should management investigate further?
The main idea was simple:

Don't just show what happened. Try to understand why it matters.

What I built
I built a 6-page interactive Power BI dashboard:

01 — Executive Overview
A quick view of the overall financial position.

It brings together:

Total Sales
Total Profit
Profit Margin
COGS
Discounts
Monthly sales trend
Segment performance
Country profitability
Product profitability
02 — Revenue & Profitability
This page focuses on revenue and profit trends.

It looks at:

Sales over time
Profit over time
Profit margin
Country revenue and profitability
Segment-level margin
03 — Business Performance
This page goes deeper into the commercial side of the business.

It looks at:

Segment performance
Profit contribution
Country-level profit
Sales mix
Monthly sales and profit
04 — Profitability Risk
This is where I moved from normal reporting into risk analysis.

It focuses on:

Discount bands
Discount exposure
Loss-making records
Loss-making products
Profitability across discount-rate bands
05 — Management Decision Center
This page is designed as a focused management view.

Instead of showing everything, it brings attention to:

Current profit margin
Discount exposure
Loss indicators
Sales mix
Product profitability
Areas that may need further investigation
06 — Global Financial Footprint
A geographic view of the financial activity in the dataset.

It shows:

Country-level sales activity
Geographic distribution
Profitability by market
Global business exposure
Key numbers from the analysis
Metric	Result
Total Sales	118.73M
Total Profit	16.89M
Profit Margin	14.23%
Total Discounts	9.21M
Loss-making records	58
Loss Record Rate	8.29%
Some findings
A few things stood out during the analysis:

Government was the strongest profit-contributing segment in the analysis.
Paseo was the highest-profit product.
France had the highest country-level profit.
Different discount bands showed clear differences in profitability.
58 records were loss-making, giving a clear area for further investigation.
These findings are based on the dataset used for this portfolio project. They should not be treated as actual company financial results.

How I built it
I followed a simple process:

1. Data cleaning
I cleaned the financial dataset before building the dashboard.

This included:

Cleaning column names
Converting dates properly
Handling missing Discount Band values
Checking duplicate records
Checking numeric fields
There were 53 missing Discount Band values. These records had zero discounts, so I classified them as No Discount instead of filling them with an arbitrary discount category.

2. Data validation
I also checked the main financial calculations:

Sales = Gross Sales − Discounts

Profit = Sales − COGS

The calculations matched the source data.

3. Data model
I created a simple dimensional model using:

FactFinancial
DimDate
DimProduct
DimCountry
DimSegment
The model was designed so that the dashboard could be filtered and analyzed across different business dimensions.

4. DAX
I created measures for:

Total Sales
Total Profit
Total COGS
Total Gross Sales
Total Discounts
Total Units
Profit Margin
Discount Rate
Financial Records
Loss Making Records
Loss Record %
Sales PY
Profit PY
Sales YoY %
Profit YoY %
Sales YTD
Profit YTD
5. Dashboard design
After validating the numbers, I designed the dashboard around the business questions.

I tried to keep the pages clean instead of adding charts just to fill space.

Tools used
Power BI
DAX
Power Query
Excel
Python
Project structure
Financial-Performance-Business-Intelligence/
│
├── README.md
│
├── data/
│   └── Financials_Cleaned.csv
│
├── powerbi/
│   └── Financial_Performance_Business_Intelligence.pbix
│
├── python/
│   └── EDA_Analysis.ipynb
│
├── screenshots/
│   ├── executive-overview.png
│   ├── revenue-profitability.png
│   ├── business-performance.png
│   ├── profitability-risk.png
│   ├── management-decision-center.png
│   └── global-financial-footprint.png
│
└── documentation/
    └── business-insights.md
What I learned
The main thing I learned from this project is that creating a chart is not the difficult part.

The difficult part is deciding:

What question should this chart answer?

While building this project, I got more comfortable with:

Data cleaning
Data validation
Dimensional modeling
DAX
Time intelligence
Financial KPIs
Profitability analysis
Risk analysis
Power BI dashboard design
Business storytelling
I also learned that a dashboard becomes much more useful when it is built around a business problem instead of just around the available columns.

Important note
This project uses a sample financial dataset for portfolio and learning purposes.

The financial figures and findings shown here are not from a real company and should not be interpreted as actual business results.

The project is intended to demonstrate my approach to data analysis, Power BI, DAX, financial reporting and business intelligence.

Links:

LinkedIn Post: https://lnkd.in/p/dJeeFbXQ 

