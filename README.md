# Atliq-Supply-Chain-Analysis
## Objective : 
To analyze and monitor the performance of a warehouse's supply chain by evaluating delivery accuracy and key performance indicators (KPIs) for 3 cities over time.
The goal is to uncover insights, inefficiencies, and support decisions for improving logistics performance.
## Problem Statement :
There have been recurring delays in customer order deliveries, accompanied by short shipments, where the delivered quantities do not match the quantities ordered.
These issues are affecting overall delivery accuracy and customer satisfaction.
## Project Overview : 
Dataset consists of 5 tables and sales data ranges from 2017 to 2020
- **1]** Customers             — City, customer_id, customer_name
- **2]** Date                  — Date, mm-yyyy,Week_No
- **3]** fact_order_lines      — Actual_Delivery_Date,Agreed_Delivery_Date,Customer_id,Delay_Days,In_Full,On_time,On Time In Full,Order_id
- **4]** Targets_Orders        — Customer_id,Infull_target%,Ontime_target%,OTIF_target%.
- **5]** Fact-orders_aggregate — Customer_id,In_full,On_time,Order_id,Order_placement_date,OTIF
- **6]** Products              - Category,Product_id,Product_Name
## Steps Involved : 
#### Data Analysis using SnowFlake
Created Database and WareHouse , Load all the requied files in stages
Connected and import data in Snowflake database and work on raw data, executed SQL commands.
### Data Cleaning and ETL(Extract, Transform, & Load)
       - Cleaning the dataset with unnecassary and duplicate records
       - Create Calculated Column for measuring KPI metrics using DAX Expersions
       - Formating the Dates in Power Query Editor 
       - Filter the required attribute in all the tables and formating the data types of the columns
       - Building relationship between tables using Data Modeling and connecting the primary key with attributes.

### Creating Report in PowerBI
   Visualizaing the data with different charts to analysis the pattern and trends in markets and working on DAX measures will provide more details insights to the stakeholders.
   ### Live Dashboard
- **Data Modeling**

<img width="1191" height="735" alt="Screenshot 2025-09-13 230414" src="https://github.com/user-attachments/assets/8fe71b08-874f-441f-986a-4426746c7518" />

- **Demagraphic Metric**

<img width="1300" height="723" alt="Screenshot 2025-09-13 223616" src="https://github.com/user-attachments/assets/3a1448ed-2cf2-4fc7-a7ea-030e05d514a8" />

- **Product Insights**

<img width="1299" height="703" alt="Screenshot 2025-09-13 223658" src="https://github.com/user-attachments/assets/879d9afc-ca46-469c-af70-76bfdc3e04b3" />

- **Delay Ratio**

<img width="1297" height="715" alt="Screenshot 2025-09-13 223750" src="https://github.com/user-attachments/assets/cb8303ae-d5c6-4287-ba0b-39dd2ba66f11" />

 ## Overview of key
- sales metrics:
- 18 Product been distributed among 35 customer in 3 cities
- **Order Delays**: 27% not delivered on time
- **Quantity Shortfalls**: 23% of ordered items undelivered
- **Delivery Failures**: 1.7% of deliveries unsuccessful*
- An average of 36% of orders fail to meet fulfillment expectations due to a combination of delivery delays and mismatched quantities.
- **Delays Rate** 1.68 Days are affected delays delivery and 13k orders are delayed over 31k orders
- **Product Delay Rate**- 66.3% of dairy product deliveries are delayed, with a maximum delay of up to 3 days


## Tools, Softwares, and Libraries
- Snowflake
- Microsoft Power BI desktop
- Power Query Editor
- DAX Language
  
       
