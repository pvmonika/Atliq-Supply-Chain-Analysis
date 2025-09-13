# Atliq-Supply-Chain-Analysis
## Objective : 
To analyze and monitor the performance of a warehouse's supply chain by evaluating delivery accuracy and key performance indicators (KPIs) for 3 cities over time.
The goal is to uncover insights, inefficiencies, and support decisions for improving logistics performance.
## Problem Statement :
There have been recurring delays in customer order deliveries, accompanied by short shipments, where the delivered quantities do not match the quantities ordered.
These issues are affecting overall delivery accuracy and customer satisfaction.
## Project Overview : 
Dataset consists of 5 tables and sales data ranges from 2017 to 2020
- **1]** Customers — City, customer_id, customer_name
- **2]** Date —      date, mm-yyyy,Week_No
- **3]** fact_order_lines — Actual_Delivery_Date,Agreed_Delivery_Date,Customer_id,Delay_Days,In_Full,On_time,On Time In Full,Order_id
- **4]** Targets_Orders — Customer_id,Infull_target%,Ontime_target%,OTIF_target%.
- **5]** Fact-orders_aggregate — Customer_id,In_full,On_time,Order_id,Order_placement_date,OTIF
- **6]** Products - Category,Product_id,Product_Name
## Steps Involved : 
#### Data Analysis using SnowFlake
Created Database and WareHouse , loading all the requied files
Connected and import data in Snowflake database and work on raw data, executed SQL commands.
### Data Cleaning and ETL(Extract, Transform, & Load)
       - Cleaning the dataset with unnecassary and duplicate records
       - Formating the currency to INR in Power Query Editor 
       - Filter the required attribute in all the tables and formating the data types of the columns
       - Building relationship between tables using Data Modeling and connecting the primary key with attributes.
       
