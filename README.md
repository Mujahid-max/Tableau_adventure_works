# Adventure Works Dashboard 📊

![dasboard perview](https://github.com/Mujahid-max/Tableau_adventure_works/blob/main/Screenshot%202025-01-22%20173920.png?raw=true)

![cycling_gif](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExcjh3b3A5c214ZDk1b2FoNDdieGY3aDdscjB2MmRmaGtieHIwcnkyMCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3o7TKVLpgWcUwpjWBG/giphy.gif)
### Overview 🏢

The Adventure Works Dashboard visualizes critical metrics for Adventure Works Cycles, a manufacturing company specializing in metal and composite bicycles. The company operates in North America, Europe, and Asia, with its headquarters in Bothell, Washington, employing 290 staff members.

This dashboard was created using Tableau, utilizing a combination of seven datasets to provide insights into sales, profit, production costs, and customer behavior. The interactive design enables users to explore data by product category, year, and country, offering a comprehensive view of business operations.
![cycling_gif](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExdHZvdDJvdnF5aHBkNTFmczV4aW03cXRiY2UxYTFmdnBrYjA4Zmd2ZyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/TfXr6aBCykBwf8ilSP/giphy.gif)
#### Data Sources 📂

The dashboard is built using the following datasets:

 * DimCustomer
* DimDate
* DimProduct
* DimProductCategory
* DimProductSubCategory
* DimSalesTerritory
* FactInternetSales (union of FactInternetSales and FactInternetSales_New)

### Data Preparation 🛠️

* Union Creation: Merged FactInternetSales and FactInternetSales_New.
### Data Enrichment:

* Used VLOOKUP to map ProductName from the DimProduct sheet to the sales data.
* Created a concatenated CustomerFullName field (First Name + Middle Name + Last Name) in DimCustomer and mapped it to the sales sheet.

##### Date Field Creation: Extracted the following fields from OrderDateKey:
* Year
* Month Number
* Month Name
* Quarter
* Year-Month
* Weekday Number
* Weekday Name
* Financial Quarter
 
### Calculated Fields:

* Sales Amount: Derived using Unit Price, Order Quantity, and Unit Discount.
* Production Cost: Computed using Unit Cost and Order Quantity.
* Profit: Calculated from Production Cost, Total Sales Amount, Tax Amount, and Freight.

### Dashboard Highlights ✨
##### Key Metrics

* Profit: $15.16M
* Sales Amount: $29.36M
* Total Production Cost: $17.28M
* Tax Amount: $2.35M

### Visualizations

* Quarterwise Sales: A pie chart displaying sales distribution across Q1, Q2, Q3, and Q4.
* Yearwise Sales: A bar chart comparing sales across different years.
* Sales and Production Cost: A combination chart showcasing trends in sales and production costs over months.
* Monthly Sales Trend: A line chart showing sales trends across months.
* Product Analysis: A table listing products with their respective profits and sales amounts.
* Customer Insights: A table highlighting customers along with their total purchases.

### Filters

* Product Category
* Year of Order Date
* Country

#### How to Use 🖱️

* Interact with filters to drill down into specific product categories, years, or countries.
* Hover over charts for detailed data insights.
* Analyze customer behavior and product performance to identify trends and opportunities.

### Conclusion 📈

This dashboard provides actionable insights for Adventure Works Cycles to enhance decision-making processes, optimize operations, and drive business growth. It demonstrates a cohesive integration of data sources and calculated metrics to deliver a comprehensive overview of the company’s performance.

