# Power BI Report Title

## Overview
This Power BI dashboard analyzes sales performance, revenue trends, customer segments, and product profitability using an anonymized dataset from the UCI Machine Learning Repository. The data itself is related to direct marketing campaigns (phone calls) of a Portuguese banking institution.

## Preview

![Home Page](Screenshot 2026-05-17 174807.png)
![Executive Summary](Screenshot 2026-05-17 174826.png)
![Customer Segment](Screenshot 2026-05-17 174840.png)
![Campaign Efficiency](Screenshot 2026-05-17 174853.png)


## Dataset

Input variables:
   # bank client data:
   1 - age (numeric)
   2 - job : type of job (categorical: "admin.","unknown","unemployed","management","housemaid","entrepreneur","student",
                                       "blue-collar","self-employed","retired","technician","services") 
   3 - marital : marital status (categorical: "married","divorced","single"; note: "divorced" means divorced or widowed)
   4 - education (categorical: "unknown","secondary","primary","tertiary")
   5 - default: has credit in default? (binary: "yes","no")
   6 - balance: average yearly balance, in euros (numeric) 
   7 - housing: has housing loan? (binary: "yes","no")
   8 - loan: has personal loan? (binary: "yes","no")
   # related with the last contact of the current campaign:
   9 - contact: contact communication type (categorical: "unknown","telephone","cellular") 
  10 - day: last contact day of the month (numeric)
  11 - month: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")
  12 - duration: last contact duration, in seconds (numeric)
   # other attributes:
  13 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
  14 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted)
  15 - previous: number of contacts performed before this campaign and for this client (numeric)
  16 - poutcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")

  Output variable (desired target):
  17 - y - has the client subscribed a term deposit? (binary: "yes","no")

  
### Additional Information

The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. 

There are four datasets: 
1) bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]
2) bank-additional.csv with 10% of the examples (4119), randomly selected from 1), and 20 inputs.
3) bank-full.csv with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs). 
4) bank.csv with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs). 
The smallest datasets are provided to test more computationally demanding machine learning algorithms (e.g., SVM). 

The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).
## Key Insights

1. Revenue increased steadily over the selected period.
2. The highest conversion job category were Students.
3. Job category management contributed the most total conversions.
4. Customer who had Tertiary education showed the strongest growth.
5. Seasonal trends were visible during March, where the most conversions happened, while the least conversions occured in May.

## Dashboard Features

- Interactive filters and slicers
- Revenue and profit KPIs
- Regional performance breakdown
- Product category analysis
- Customer segment analysis
- Time series trend charts
- Drill through or tooltip pages

## Tools Used

- Power BI Desktop
- Power Query
- DAX
- CSV
- GitHub

## Power BI Techniques Used
- Data cleaning in Power Query
- Relationship modeling
- DAX measures
- Calculated columns
- KPI cards
- Slicers and filters
- Drill through pages
- Custom tooltips
- Conditional formatting

## How to Use This Report

1. Download the `.pbix` file from the `report/` folder.
2. Open it in Power BI Desktop.
3. If needed, update the data source path.
4. Refresh the data.
5. Explore the report pages and filters.
