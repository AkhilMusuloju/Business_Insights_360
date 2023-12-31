# Business_Insights_360

## **Project Overview:**

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.


_[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiNDA3MTk5YTgtNGI2NC00NWFiLWE0YTUtMDQ0NzhiODA0ZWQ2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)_

## **Tools used:**

- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## **PowerBI techniques Learnt:**

- What are all the questions should be asked before staring the project
- Creating calculated columns
- creating measure using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- PowerBi services
- Publishing reports to PowerBi services
- Setting up personal gateway to set up the auto refresh of data
- PowerBi App creation
- Collaboration, workspace, access permissions in PowerBi services
And more

## **Business related terms:**
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
## **Company’s back ground:**
  
AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel

- Retailers
- Direct
- Distributors
  
Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry.

Project kick off session, where you should get clear of for what and why this project and all other questions you have with regards to the project

## **Questions to ask before starting with dashboard:**
- What is the objective of building this PowerBi dashboard?
- In what terms the success of this project will be measured?
- What will be time dead-line of the project?
- do the stakeholders expecting pre-view before the actual release?
- What are all the hopes stakeholders have out of this project?
- what are all fears the stakeholder have in terms of building this dashboard?
- Who are all will be using this dashboard and for what purpose?
- what are all expectation the stakeholders have, by the completion of this project?
- What can go wrong while building this project?
- what are all the resources/ data needed to build this dashboard?
- is there any inputs from stakeholders in terms of design and views of the dashboard?
  
After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

## **Dataset Understanding:**
Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions

## **gdb041:**
dim_customer
- 27 distinct markets (ex India, USA, spain)
- 75 distinct customers thorough out the market
- 2 types of platforms
     - Brick & Motors - Physical/offline store
     - E-commerce - Online Store (Amazon, flipkart)
- Three channels
     - Retailer
     - Direct
     - Distributors

**dim_market:**
- 27 distinct markets (ex India, USA, spain)
- 7 sub-zones
- 4 regions
     - APAC
     - EU
     - nan
     - LATAM

**dim_product:**
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
  
**fact_forecast_monthly:**
- This table is used to forecast the customer’s need in advance, which can help in
    - Higher customer satisfaction
    - Reduced cost in warehouses for storage purpose
- The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
- All the date of the month will be replaced by the start date of the month
- It will have all the column names and in the end it will have the forecast quantity need of the customer
  
**fact_sales_monthly:**
- This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
  
## **gdb056**

freight_cost
- This table has details of travel cost and other cost for each market with fiscal year
gross_price
- Has the details of gross prices with product code
manufacturing_cost
- Has the details of manufacturing cost with product code with year
Pre_invoice_dedutions
- Has the details of pre invoice deductions percentage for each cutomer with year
Post_invoice_deductions
- Post invoice deductions and other deductions details
  
## **Importing data into PowerBi:**

As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential
Data Model

Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.

Poor data modeling affects the over all performance of the report.

Following Good practices of data modeling is must.

In this project, we have followed Snowfall data modeling method.

<img width="582" alt="Screenshot 2023-10-03 191958" src="https://github.com/AkhilMusuloju/Business_Insights_360/assets/142907602/b4baff97-6ef9-44cc-93cf-8f59812ce70c">

## **Dashboard designing:**
Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required


## **Home view**

In Home view, all the views button will be available. User will land on specific view page by clicking the button

**Info**
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Support
<img width="518" alt="Home" src="https://github.com/AkhilMusuloju/Business_Insights_360/assets/142907602/8881e840-73c2-4d15-a926-7222131933a0">

## Finance View
<img width="558" alt="Finance View" src="https://github.com/AkhilMusuloju/Business_Insights_360/assets/142907602/4e395766-b093-4b08-a06f-4784305e0cfd">

## Sales View
<img width="558" alt="Sales View" src="https://github.com/AkhilMusuloju/Business_Insights_360/assets/142907602/8cd56d9c-1f8f-4fac-8d40-bf632803db33">

## Marketing View
<img width="559" alt="Markeng View" src="https://github.com/AkhilMusuloju/Business_Insights_360/assets/142907602/98d0233e-1020-41ac-9490-9f3b2b582cff">

## Supply chain View
<img width="558" alt="Supply Chain View" src="https://github.com/AkhilMusuloju/Business_Insights_360/assets/142907602/32b7db0c-fb67-4e56-bb79-f4bf42a5c91c">

## Executive View
<img width="579" alt="Executive View" src="https://github.com/AkhilMusuloju/Business_Insights_360/assets/142907602/f3527c76-043b-4d65-9285-a4ba8aa0b3cd">


## **Project Outcome**

By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
