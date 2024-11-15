# Business-Insights-360
## Project Overview

AtliQ Hardware has been growing rapidly in recent years, and they have decided to implement data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data-driven decisions. This project is hoped to give answers to the questions of stakeholders in terms all aspects like finance, sales, marketing, and supply chain.

I worked on this project by following the Codebasics PowerBi Course, Link to the course is [here](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)

[Live Report Link](https://www.novypro.com/project/atliq-hardware-business-insights-360)

## Tech stacks

- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## PowerBI techniques Learnt

- What are all the questions that should be asked before starting the project
- Creating calculated columns
- creating measures using the DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using the divide function to prevent zero division errors
- creating data table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting of the values in visuals using icons or background color
- Data validation techniques
- PowerBi services
- Publishing reports to PowerBi services
- Setting up a personal gateway to set up the auto-refresh of data
- PowerBi App creation
- Collaboration, workspace, and access permissions in PowerBi services
- And more 😅

## GitHub 

- Uploading Large size files using GitHub LFS
- Tracking the particular type of file extensions for LFS

## Business related terms

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## Company’s background

AltiQ Hardware is a company that has grown vastly in recent years, and opened business all over the globe. It is a company that sells computers and computer accessories through three mediums/channel

- Retailers
- Direct
- Distributors

Recently, the company faced an unforeseen loss by opening a store in America based on surveys, intuition, and some Excel analysis. Also, the company’s competitors have a handful of analytics teams to perform analysis and make data-driven decisions. So, AltiQ Hardware has no other option than building its analytics team for data-driven insights and decisions in the future to survive better in the industry. 

Project kick-off session, where you should get clear of what and why this project is and all other questions you have with regards to the project

### Questions to ask before starting with the dashboard

- What is the objective of building this PowerBi dashboard?
- In what terms will the success of this project be measured?
- What will be the deadline of the project?
- Are the stakeholders expecting a preview before the actual release?
- What are all the hopes stakeholders have out of this project?
- what are all the fears the stakeholders have in terms of building this dashboard?
- Who will be using this dashboard and for what purpose?
- what are all expectations the stakeholders have, by the completion of this project?
- What can go wrong while building this project?
- what are all the resources/ data needed to build this dashboard?
- Is there any input from stakeholders in terms of design and views of the dashboard?

After the project kick-off meetings, the data engineering team has given the data as per the request of the data analytics team, let’s explore them.

### Dataset **Understanding.**

Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get a good understanding of what are data available.

Dimension table: It will have static data like details of customers and products

Fact table: It will have the data about the transactions  

- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, Spain)
        - **75** distinct customers throughout the market
        - **2** types of platforms
            - Brick & Motors - Physical/offline store
            - E-commerce - Online Store (Amazon, Flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, Spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s needs in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purposes
        - The table is denormalized by the data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
        - All the dates of the month will be replaced by the start date of the month
        - It will have all the column names and in the end, it will have the forecast quantity needed of the customer
    - fact_sales_monthly
        - This table is more or less is same as the fact_forecase_monthly table, but the last column has the value of the sold quantity instead of the forecast value.
- gdb056
    - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
        - Has the details of gross prices with product code
    - manufacturing_cost
        - Has the details of manufacturing cost with product code with year
    - Pre_invoice_dedutions
        - Has the details of pre-invoice deductions percentage for each customer with year
    - Post_invoice_deductions
        - Post invoice deductions and other deduction details

## Importing data into PowerBi

- As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential

## Data Model

- Data modeling plays a vital role and is considered as the basement of the report. All the visuals will be built upon the data model.
- Poor data modeling affects the overall performance of the report.
- Following Good practices of data modeling is a must. Refer to this page to get to know the good practices [Blog](https://addendanalytics.com/blog/data-modelling-best-practices/)
- In this project, we have followed the Snowfall data modeling method.

<img src="https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Data_model.png" class="center">

### Dashboard designing

Based on the mock-ups received as a requirement, the team will start designing the visuals and create measurements as and when required

## Home view

In-Home view, all the views button will be available. Users will land on a specific view page by clicking the button 

- Info
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Products
- Support

## Overall Report

![Overall Report.gif](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Overall.gif)

## Info Page

![Info.gif](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Info.gif)

## Finance View

![Finace.gif](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Finace.gif)
## Sales View

![Sales.gif](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Sales.gif)

## Marketing View

![Marketing.gif](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Marketing.gif)

## Supply chain View

![Supply chain.gif](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/supply%20chain.gif)

## Executive View

![Executive.gif](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Executive.gif)

## Products

![Products](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Products%20View.gif)

you can find the full report file here : [Report](https://github.com/Naveen-S6/Business_Insights_360/blob/main/Report/360.pbix)


## Project Outcome

By using this report, decisions can be made based on the data. Further, it will help in answering n number of why questions based on the situation.
