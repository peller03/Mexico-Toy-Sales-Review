# Mexico-Toy-Sales-Review
---
## Table of Contents
- [Project Scope](#project-scope)
- [Data Sources](#data-sources)
- [Tool Used](#tool-used)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Exploratory Data Analysis Performed](#exploratory-data-analysis-performed)
- [EDA Visual Insights](#eda-visual-insights)
- [ Data Analysis](data-analysis)
- [Results / Findings](results-findings)
- [Recommendations](recommendations)
- [Limitations](limitation)

### Project Scope
This project analyzes toy sales trends across Mexico using Power BI. The goal is to understand revenue drivers, top-performing products, regional sales differences, and seasonal patterns.
The dashboard provides insights to help retailers optimize inventory, improve marketing strategy, and boost profitability.


![P11_P12_P13](https://github.com/user-attachments/assets/ad4e483d-f864-4f78-9ce3-36b1d1745eda)

### Data Sources
The dataset was sourced from Maven Analytics, containing structured sales records with one fact table (Sales) and four dimension tables (Product, Store, Inventory, Calendar).

Supporting files include:
-  calender.csv
  
-  sales.csv
  
-  inventory.csv
  
-  products.csv
  
-  data_dictionary.csv
  
### Tool Used

- Microsoft Power BI – Data cleaning, modeling, DAX calculations, and dashboard design
  
- Power Query – Transformation, data type correction, and table formatting
  
- DAX – KPI calculations (SUM, AVERAGE, COUNT)
 
### Data Cleaning & Preparation

1. Clean currency values by removing $ symbols and converting to Fixed Decimal Number.
2. Fix date format issues in the Calendar table using "Change Type → Using Locale" (EN-US).
3. Check for missing values using Power Query column quality indicators.
4. Resolve many-to-many relationship between Sales and Inventory by creating a unique concatenated key (Inventory ID).
5. Improve date readability by creating short month and day columns (Jan–Dec, Mon–Sun).

### Exploratory Data Analysis Performed

The EDA focused on major KPIs and performance patterns. Key KPIs include:
- Total Revenue: $14.4M
  
- Total Profit: $4.01M
  
- Average Selling Price: $13.245
  
- Total Orders: 829k
  
- Top Product Category: Lego Brick

### EDA Visual Insights:
- Lego Bricks leads revenue with ~$2M.
  
- April is the peak revenue month (~$1.5M).
  
- Toys Cuidad de Mexico 2 sold the highest quantity (~43K units).
  
- Toys Guadalajara is the top revenue-generating city.

### Data Analysis
Using DAX:
- SUM was used for total revenue/profit.
- AVERAGE computed the average selling price.
- COUNT identified 50 unique stores.

- Key Findings:
  - Revenue is driven by urban store locations.
    
  - Product categories like Lego Bricks and Toys & Crafts dominate revenue.
    
  -  Weekly performance is consistent, with mid-week sales peaks.
 
### Results / Findings
From the dashboard:

- Total revenue: $14.4M, profit: $4.01M

- Lego Bricks = highest revenue category ($5.1M)
  
- April = highest sales month
  
- Toys Guadalajara = highest revenue city
  
- Toys Cuidad de Mexico 2 = highest quantity sold (43k)

### Recommendations
Based on insights:
1. Increase stock for high-demand products like Lego Bricks.
2. Invest more in high-performing urban cities such as Guadalajara.
3. Align promotions with seasonal peaks (especially April).
4. Optimize inventory allocation based on store performance differences.

### Limitations
1. The dataset does not include customer demographics.
2. No competitive or pricing comparison with other retailers.
3. External factors behind seasonal spikes are not provided.
