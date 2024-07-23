# AtliQ Hardware-Sales & Finance Analytics 

## AtliQ Hardware Business Model:

*AtliQ is a hardware company which sells hardware such as keyboards,mouse,PC,printers etc to consumers.

*AtliQ Hardware sends their products to Warehouses and which is shipped to various locations.

*AtliQ's products are avilable through platforms like Croma, Best Buy (Brick & Mortar) and Amazom (E-Commerce)

*AtliQ has their own store - AtliQ Exclusive and AltiQ e store

*AtliQ distributes through 3 channels - Retailer,Direct Stores,Distributor

## Business Requirement:

 Atliq Hardware is a company moving towards advanced analytics.Create Sales and Finance Analytics Report for data-informed decision making

## Why the need for Sales Analytics Report

*To analyse discounts,promotions and performance bonus to retailers/customers

*To expand the purchase to various locations based on sales.If a product is performing well in a particular region then expansion of store can be considered in that region

## ETL in Excel:

![Screenshot 2024-07-22 205128](https://github.com/user-attachments/assets/06025cf6-3c10-4a6d-abcc-2e86304534a6)

## Data Source : CSV files

## Data Transformation :

1.Use First Row as Headers

2.Check for errors using Column distribution and Column quality option - **dim_customer,dim_market,dim_product ,fact_sales_monthly**

3.Check for duplicates by looking at the unique and distinct values in all dimension tables.For example: dim_customer table has customer_code which is a primary key and should not contain duplicates

4.Replaced mispelled customer_name in dim_customer table 

5.Replaced values in market column 'nan' with 'NA' in dim_market table

6.Replaced negative quantity values by using absolute option

## Creating plan for report creation:

![Screenshot 2024-07-23 124643](https://github.com/user-attachments/assets/0d560dfc-1f65-429b-a372-95a88919114d)

Listing the componenets:

1.Net Sales

2.Year

3.Division

4.Region

5.Country

## Data Modelling:

Connecting primary keys of dimension tables with the foreign keys of fact tables

![Screenshot 2024-07-23 130821](https://github.com/user-attachments/assets/96f59320-9c08-4381-8961-272ab8a3c73c)

-Created dim_date table (Fiscal_year) and connected to fact table 
  *Used Date.Addmonth() and Date.year() funcions to add 4 months to get the respective fiscal year and to extract year from the date respectively

 ## Project objective:

  **1.** Create a _[Customer Performance Report](https://github.com/ErnestaRoschelle/Sales-Analytics-Business-Report/blob/main/customer%20performance%20net%20sales.pdf)_
  
  **2.** Conduct a comprehensive comparison between _[market performance and sales target](https://github.com/ErnestaRoschelle/Sales-Analytics-Business-Report/blob/main/Market%20Performance%20report.pdf)_
  
  **3.** To find out the _[top 10 selling products](https://github.com/ErnestaRoschelle/Sales-Analytics-Business-Report/blob/main/top%2010%20products.pdf)_
  
  **4.** To find out _[top 5 products and bottom 5 products](https://github.com/ErnestaRoschelle/Sales-Analytics-Business-Report/blob/main/Top%205%20%26%20bottom%205%20products.pdf)_
  
  **5.** To examine [new products-2021](https://github.com/ErnestaRoschelle/Sales-Analytics-Business-Report/blob/main/New%20products%202021.pdf)
  
  **6.** To find out the performance of _[sales Division wise](https://github.com/ErnestaRoschelle/Sales-Analytics-Business-Report/blob/main/Division%20level%20report.pdf)_
  
  **7.** To find out _[top 5 performing countries](https://github.com/ErnestaRoschelle/Sales-Analytics-Business-Report/blob/main/top%205%20countries.pdf)_

## Steps Involved in building this report:

1.Data Extraction 

2.Data Transformation in Power Query Editor

3.Data Loading 

4.Building Mock up Report

5.Listing the components from the Mock up Report

6.Tangible Action Points

7.Data Modelling in Power Pivot

8.Building Report in Pivot Table using DAX

9.Beautify the Report for User Readability using Conditional Formatting


