# Business-Insights-360

Welcome to the AtliQ Hardware Data Analytics Project Repository. In this project I have used MySQL to generate insightful reports.

## Project Overview
In this project, we have implemented data analytics using Power BI to empower AtliQ Hardware with the ability to make data-driven decisions, surpass competitors in the market, and drive growth in various aspects of their business, including finance, sales, marketing, and supply chain management.

## Introduction

## Tech Stacks
1. SQL
2. Excel
3. Power BI
4. DAX Language
5. DAX Studio

## Business Terminology

1. **Gross Price**: The total price of a product or service before any deductions, such as taxes or discounts, are applied.

2. **Pre-Invoice Deductions**: Deductions made from the gross price before an invoice is generated. These could include discounts, allowances, or other adjustments.

3. **Post-Invoice Deductions**: Deductions made after an invoice is generated. These deductions might involve returns, rebates, or adjustments that affect the final amount the customer pays.

4. **Net Invoice Sale**: The final amount after deducting both pre-invoice and post-invoice deductions from the gross price.

5. **Gross Margin**: The difference between the revenue generated from sales and the cost of goods sold (COGS). It indicates how much profit a company makes from its core business operations.

6. **Net Sales**: The total revenue generated from sales after deducting returns, allowances, and discounts.

7. **Net Profit**: The total profit a company earns after deducting all expenses, including COGS, operating expenses, and taxes, from its total revenue.

8. **COGS (Cost of Goods Sold)**: The direct costs associated with producing the goods that a company sells. It includes the cost of raw materials, labor, and manufacturing overhead.

9. **YTD (Year to Date)**: Refers to the period starting from the beginning of the current calendar year up to the present date. It's often used to analyze performance or financial metrics within a specific timeframe.

10. **YTG (Year to Go)**: Refers to the remaining period in the current calendar year, starting from the present date and extending until the end of the year.

11. **Direct**: A sales channel where products are sold directly from the manufacturer or company to the end consumer without intermediaries.

12. **Retailer**: An entity that purchases products from manufacturers or wholesalers and sells them to consumers, often through physical or online stores.

13. **Distributors**: Entities that purchase products in bulk from manufacturers and then sell them to retailers or other businesses. They help bridge the gap between manufacturers and retailers.

14. **Consumer**: The end-user or customer who purchases and uses the products or services offered by a company.

## Company's Background

AtliQ Hardware is a rapidly growing company that specializes in selling computers and computer accessories through three primary channels:

1. Retailers
2. Direct Sales
3. Distributors
   
With a global presence, the company has expanded its business operations significantly in recent years.

## Dataset

## Dimension Tables

**dim_customer**

* Contains details of customers across markets and platforms.
* 27 distinct markets.
* 75 distinct customers.
* 2 types of platforms: Brick & Mortar (Physical/offline store) and e-commerce (Online Store).
* Three channels: Retailer, Direct, and Distributors.
  
**dim_market**

* Contains details of markets, sub-zones, and regions.
* 27 distinct markets.
* 7 sub-zones.
* 4 regions: APAC, EU, NA, LATAM.
  
**dim_product**

* Contains details of product divisions, categories, and variants.
* Divisions: P & A, Peripherals, Accessories, PC, Notebook, Desktop, N & S, Networking, Storage.
* 14 different categories (e.g., Internal HDD, keyboard).
* Different variants available for the same product.
  
**Fact Tables**

* fact_forecast_monthly
* Used for forecasting customer needs in advance.
* Helps improve customer satisfaction and reduce warehouse storage costs.
* Denormalized for analytical use.
* Date of the month replaced by start date.
* Columns include forecast quantity needed by the customer.
  
**fact_sales_monthly**
  
* Similar to fact_forecast_monthly with actual sold quantities.

**Additional Tables**
  
 **gdb056 **
 
1. **freight_cost**: Details of travel and other costs for each market by fiscal year.

2. gross_price Details of gross prices with product code.

3. **manufacturing_cost**: Details of manufacturing costs with product code and year.

4. **Pre_invoice_dedutions**: Details of pre-invoice deduction percentages for each customer by year.

5. **Post_invoice_deductions**: Details of post-invoice and other deductions.

This dataset provides comprehensive information about customers, markets, products, and various costs. The dimension tables offer static data, while the fact tables provide transactional and forecasting insights. Analyzing this dataset can lead to valuable insights for optimizing sales, costs, and customer satisfaction.

**Data Model**

Data modelling plays a pivotal role and serves as the foundation for generating meaningful reports. The entire framework of visualizations is constructed upon a well-designed data model. Neglecting proper data modelling can have adverse effects on the overall performance of the generated reports.

In the context of this project, we have meticulously followed the Snowflake data modelling method. This approach involves structuring data into normalized forms, resulting in reduced redundancy and improved query performance. This methodology enhances the way we organize and process data, ensuring optimal results for our analysis.

![Screenshot 2024-05-08 113546](https://github.com/Kartiksinghbisen/Business-Insights-360/assets/139736045/aa2d0544-be3e-44be-94fc-8e316c70c404)




## Dashboard

You can find the Interactive Dashboard [here](https://app.powerbi.com/view?r=eyJrIjoiMmM3MDE2M2ItZGZjZC00ZWEwLWEzMjItOGY0NWJiNWMyMzRlIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## HOME VIEW
![Screenshot 2024-05-08 113329](https://github.com/Kartiksinghbisen/Business-Insights-360/assets/139736045/877570bf-5eb9-4cc7-8a63-95961bd9fb56)


## FINANCE VIEW
![Screenshot 2024-05-08 113411](https://github.com/Kartiksinghbisen/Business-Insights-360/assets/139736045/4ed304a4-5d06-420d-ad9a-b85a3eb5249a)


## SALES VIEW

![Screenshot 2024-05-08 113432](https://github.com/Kartiksinghbisen/Business-Insights-360/assets/139736045/79808b94-1f1b-4a7d-b0a5-9e50082e82d5)

## SUPPLY CHAIN VIEW
![Screenshot 2024-05-08 113451](https://github.com/Kartiksinghbisen/Business-Insights-360/assets/139736045/46997f1b-d864-4787-9394-7c177bd7e7bf)

## MARKETING VIEW
![Screenshot 2024-05-08 113509](https://github.com/Kartiksinghbisen/Business-Insights-360/assets/139736045/8fc76dd8-a8ba-409a-89d0-7e676d953c04)



## EXECUTIVE VIEW
![Screenshot 2024-05-08 113524](https://github.com/Kartiksinghbisen/Business-Insights-360/assets/139736045/e3e3912a-8675-4ecf-b668-07cf87326deb)
