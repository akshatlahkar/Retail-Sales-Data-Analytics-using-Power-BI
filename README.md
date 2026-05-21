# Retail-Sales-Data-Analytics-using-Power-BI
Interactive Retail Sales Dashboard built using Power BI to analyze sales, profit, product performance, discounts, and customer transactions. Implemented Star Schema data modeling, Power Query transformations, Top/Bottom analysis, trend analysis, map visuals, and interactive comparison dashboards.



## Problem Statement

This dashboard helps businesses analyze their retail sales performance better. It helps them identify top and bottom performing products based on sales, profit & quantity sold. Through different visualizations and analytical pages, businesses can understand sales trends over time, relationship between sales & profit, impact of promotional discounts and geographical sales distribution across different cities.

It also lets businesses compare total sales, total profit & quantity sold between two selected periods using interactive slicers. Thus, by using this dashboard they can identify product performance, promotional effectiveness and overall sales trends.

Since the project uses a Star Schema data model consisting of one fact table and multiple dimension tables, report filtering and analysis become more efficient and scalable.

Also since comparison analysis was implemented using synchronized slicers & edit interactions instead of DAX based calculations, users can interactively compare two different periods in a simpler manner.


### Steps followed 


- Step 1 : Power Query Editor was used to analyze column quality, column distribution & column profile for complete dataset validation.

- Step 2 : Data types, distinct values, unique values, empty values & errors were checked across all tables.

- Step 3 : A Star Schema data model was created consisting of:
  
  (a) Fact Table
  
  (b) Dim Customers
  
  (c) Dim Product
  
  (d) Dim Promotion

- Step 4 : One-to-many relationships were created between fact & dimension tables using primary and foreign keys.

- Step 5 : Promotion categories were transformed into numerical percentage values using conditional columns in Power Query.

- Step 6 : Merge Queries operations were used to populate missing fields such as:
  
  (a) Price Per Unit
  
  (b) Discount Percentage

- Step 7 : Custom columns were created to calculate:
        
        Total Sales = [Unit Sold] * [Price Per Unit]

        Profit = 0.1 * [Net Sales]

- Step 8 : Null values in discount percentage column were replaced with zero using Replace Values transformation.

- Step 9 : A report page named "Top Bottom Five Analysis" was created.

- Step 10 : Stacked bar charts were added to represent:
  
  (a) Top 5 Products by Sales
  
  (b) Bottom 5 Products by Sales
  
  (c) Top 5 Products by Profit
  
  (d) Bottom 5 Products by Profit
  
  (e) Top 5 Products by Quantity Sold
  
  (f) Bottom 5 Products by Quantity Sold

- Step 11 : Top N & Bottom N filters were applied to dynamically represent top and bottom performing products.

- Step 12 : A separate "Overview" dashboard page was created for analytical visualizations.

- Step 13 : Line chart with drill up & drill down functionality was added to analyze sales trends over yearly, quarterly, monthly & daily periods.

- Step 14 : Scatter plot was added to represent relationship between Profit & Net Sales.

- Step 15 : Bar chart was added to analyze average discount offered under different promotion categories.

- Step 16 : Map visual was added to represent sales distribution across different cities.

- Step 17 : A separate comparison dashboard page was created using two independent date slicers.

- Step 18 : Bar charts were added to compare:
  
  (a) Total Sales
  
  (b) Total Profit
  
  (c) Total Quantity Sold

between two selected periods.

- Step 19 : Edit Interactions functionality was used to control slicer interaction behaviour between visuals.

- Step 20 : A transaction level filter dashboard page was created using table visuals.

- Step 21 : Table visual was used to represent:
  
  (a) Customer ID
  
  (b) Order ID
  
  (c) Product ID
  
  (d) Promotion ID
  
  (e) Discount
  
  (f) Discount Percentage
  
  (g) Net Sales
  
  (h) Price Per Unit
  
  (i) Profit
  
  (j) Total Sales
  
  (k) Units Sold

- Step 22 : Visual filters (Slicers) were added for:
  
  (a) Date
  
  (b) Customer Name
  
  (c) Product Name
  
  (d) Promotion Name

- Step 23 : Different formatting operations were performed including:
  
  - Borders
  
  - Data labels
  
  - Gridline customization
  
  - Font formatting
  
  - Visual resizing
  
  - Color customization

- Step 24 : The report was then saved on Power BI Service.


# Snapshot of Dashboard (Power BI Service)


![Dashboard_1](Screenshot%20(179).png)

![Dashboard_2](Screenshot%20(180).png)

![Dashboard_3](Screenshot%20(181).png)

![Dashboard_4](Screenshot%20(182).png)

![Dashboard_5](Screenshot%20(184).png)
 


# Insights

A multi page interactive retail sales dashboard was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Product Performance Analysis

   Top performing products were identified using sales, profit & quantity sold metrics.

   Bottom performing products were also analyzed using Bottom N filtering.

   Product performance varied significantly across different metrics.


### [2] Sales Trend Analysis

   Sales trends were analyzed over yearly, quarterly, monthly & daily periods.

   Drill down functionality enabled detailed hierarchy based analysis.


### [3] Profit vs Net Sales Analysis

   Positive relationship between Profit & Net Sales was observed using scatter plot analysis.

   Majority of transactions were concentrated within lower sales & lower profit ranges.


### [4] Promotion Analysis

   Average discount offered under different promotion categories was analyzed.

   Blank promotion category represented transactions where no discount was applied.


### [5] Geographical Analysis

   Sales across different cities were represented using map visuals.

   Cities with larger bubble sizes contributed higher sales values.


### [6] Comparison Dashboard Analysis

   Users can compare total sales, total profit & total quantity sold between two different periods.

   Comparison analysis was implemented using synchronized slicers & edit interactions instead of DAX based calculations.


### [7] Transaction Level Analysis

   Transaction level filtering was implemented using slicers from multiple dimension tables.

   Users can dynamically filter records using:
   
   (a) Date
   
   (b) Customer Name
   
   (c) Product Name
   
   (d) Promotion Name


### [8] Data Modeling

   Star Schema implementation improved report organization & filtering efficiency.

   One-to-many relationships enabled scalable & optimized report analysis.
