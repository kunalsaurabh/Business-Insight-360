# Business Insights 360 - Project Summary

## Project Overview

AtliQ Hardware, a rapidly growing company, has initiated a data analytics project using PowerBI to gain a competitive edge and make data-driven decisions. This project aims to provide stakeholders with insights across finance, sales, marketing, and supply chain.

 **Live Report:** [AtliQ Hardware Business Insights 360](https://app.powerbi.com/view?r=eyJrIjoiY2JlY2UyZGYtOGNmYS00NzVjLThjOTYtM2Q1MmYyNTY3YmU3IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Technologies Used

- **SQL**
- **PowerBI Desktop**
- **Excel**
- **DAX Language**
- **DAX Studio** (for report optimization)
- **Project Charter**

## Key Skills and Techniques Acquired

- **Requirement Analysis:**
  - Identifying project objectives
  - Defining success metrics
  - Understanding stakeholder expectations
- **Data Modeling:**
  - Implementing Snowflake schema
  - Best practices for efficient data modeling
- **DAX Language Proficiency:**
  - Creating calculated columns and measures
  - Utilizing divide function to prevent zero-division errors
- **Advanced PowerBI Features:**
  - Bookmarks for visual switching
  - Page navigation with buttons
  - Dynamic titles based on filters
  - Conditional formatting using icons or background color
  - KPI indicators and data validation
- **PowerBI Services:**
  - Report publishing
  - Setting up auto-refresh with personal gateway
  - Creating and managing PowerBI apps
  - Collaboration, workspace management, and access permissions
- **GitHub:**
  - Managing large files with GitHub LFS

## Business Acumen

- **Financial Metrics:**
  - Gross Price, Net Sales, Gross Margin, Net Profit
- **Sales and Marketing Metrics:**
  - YTD (Year to Date), YTG (Year to Go)
- **Supply Chain Insights:**
  - Cost of Goods Sold (COGS)
- **Customer and Market Analysis:**
  - Understanding different sales channels (Retailers, Direct, Distributors)
  - Analyzing market and customer data

## Company Background

**AtliQ Hardware** is a global company selling computers and accessories through various channels. Faced with a recent setback in the American and other markete, the company is building an analytics team to drive data-driven decisions and improve market positioning.

### Essential Questions for Dashboard Development

- What are the project objectives and success metrics?
- What is the project deadline?
- Are stakeholders expecting a preview before the final release?
- Who are the end-users of the dashboard and their requirements?
- What resources and data are needed?
- Are there specific design and view preferences from stakeholders?


## Dataset Understanding

Understanding the available data is crucial for effective analysis. Before diving into the analysis, it is important to get a clear understanding of the data available.

### Dimension Tables

Dimension tables contain static data such as customer and product details.

**Database: gdb041**

- **dim_customer table**
  - 27 distinct markets (e.g., India, USA, Spain)
  - 75 distinct customers throughout the markets
  - 2 types of platforms:
    - Brick & Mortar - Physical/offline store
    - E-commerce - Online Store (Amazon, Flipkart)
  - Three channels:
    - Retailer
    - Direct
    - Distributors

- **dim_market table**
  - 27 distinct markets (e.g., India, USA, Spain)
  - 7 sub-zones
  - 4 regions:
    - APAC
    - EU
    - NA
    - LATAM

- **dim_product table**
  - Divisions:
    - P & A
      - Peripherals
      - Accessories
    - PC
      - Notebook
      - Desktop
    - N & S
      - Networking
      - Storage
  - 14 different categories (e.g., Internal HDD, Keyboard)
  - Various product variants available

### Fact Tables

Fact tables contain transactional data.

**Database: gdb041**

- **fact_forecast_monthly table**
  - Forecasts customer needs in advance to help with:
    - Higher customer satisfaction
    - Reduced warehouse storage costs
  - Denormalized by the data engineering team for analytical use
  - All dates in the month are replaced by the start date of the month
  - Contains all column names and the forecast quantity needed by the customer

- **fact_sales_monthly table**
  - Similar to the fact_forecast_monthly table but contains sold quantity instead of forecast value

**Database: gdb056**

- **freight_cost table**
  - Contains travel cost and other costs for each market with the fiscal year

- **gross_price table**
  - Contains details of gross prices with product code

- **manufacturing_cost table**
  - Contains details of manufacturing costs with product code and year

- **Pre_invoice_deductions table**
  - Contains details of pre-invoice deductions percentage for each customer with year

- **Post_invoice_deductions table**
  - Contains details of post-invoice deductions and other deductions


### Data Import and Model

- **Data Import:** Importing data from MySQL to PowerBI
- **Data Model:** Following Snowflake schema for efficient data modeling

![Data Model](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Model%20View.png)

### Dashboard Design and Home View

**Home View:** Centralized view with navigation buttons to different sections
![Home-page.gif](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Home-page.gif)

- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Support

## Finance View

![Finance.gif](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Finance.gif)

## Sales View

![Sales.gif](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Sales.gif)

## Marketing View

![Marketing.gif](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Marketing.gif)

## Supply chain View

![Supply-Chain.gif](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Supply-Chain.gif)

## Executive View

![Executive.gif](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Executive.gif)

## Products

![Support.gif](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/Resource/Support.gif)

Click here to find the complete BI report : [Report](https://github.com/kunalsaurabh/Business-Insight-360/blob/main/BI%20Report/Business_Insights.pbix)

## Conclusion

This project enabled me to develop a comprehensive PowerBI dashboard providing actionable insights for AtliQ Hardware. I gained valuable experience in advanced PowerBI features, data modeling, DAX language, and understanding business metrics, positioning me well for roles in data analysis and business intelligence.
