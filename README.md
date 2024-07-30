# Business-Insights-360
 **Project Overview:**  
 AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBI in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

## Tech stacks
- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file
## PowerBI Techniques Learnt
- What are, all the questions should be asked before staring the project
- Creating calculated columns
- Creating measure using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- Creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- PowerBI services
- Publishing reports to PowerBI services
- Setting up personal gateway to set up the auto refresh of data
- PowerBI App creation
- Collaboration, workspace, access permissions in PowerBI services
And more 😅
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
## Company’s Background
- AtliQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel.
- Retailers
- Direct
- Distributors
- Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry.
- Project kick off session, where you should get clear of for what and why this project and all other questions you have, with regards to the project.
## Questions to ask before starting with dashboard
- What is the objective of building this PowerBI dashboard?
- In what terms the success of this project will be measured?
- What will be time dead-line of the project?
- Do the stakeholders expecting pre-view before the actual release?
- What are all the hopes stakeholders have out of this project?
- What are all fears that stakeholder have in terms of building this dashboard?
- Who are all will be using this dashboard and for what purpose?
- What all expectation the stakeholders have, by the completion of this project?
- What can go wrong while building this project?
- What are all the resources/ data needed to build this dashboard?
- Are there any inputs from stakeholders in terms of design and views of the dashboard?
- After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.
## Dataset Understanding.
- Understanding what data is available will be more helpful while doing analysis. Before jumping on to the analysis gets good understanding of what are data available.

Dimension Table : It will have the static data like details of customer and products.

Fact Table : It will have the data about the transactions.
#### gdb041:
###### dim_customer
- 27 distinct markets (ex India, USA, spain)
- 75 distinct customers thorough out the market
- 2 types of platforms
- Brick & Motors - Physical/offline store
- E-commerce - Online Store (Amazon, flipkart)
- Three channels
- Retailer
- Direct
- Distributors
###### dim_market
- 27 distinct markets (ex India, USA, spain)
- 7 sub-zones
- 4 regions
- APAC
- EU
- NAN
- LATAM
###### dim_product
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
###### fact_forecast_monthly
- This table is used to forecast the customer’s need in advance, which can help in
- Higher customer satisfaction
- Reduced cost in warehouses for storage purpose
- The table is DE normalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
- All the date of the month will be replaced by the start date of the month
- It will have all the column names and in the end it will have the forecast quantity need of the customer
###### fact_sales_monthly
- This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
###### gdb056
- Freight_Cost
- This table has details of travel cost and other cost for each market with fiscal year
- Gross_Price
- Has the details of gross prices with product code
- Manufacturing_Cost
- Has the details of manufacturing cost with product code with year
- Pre_Invoice_Dedutions
- Has the details of pre invoice deductions percentage for each cutomer with year
- Post_invoice_deductions
- Post invoice deductions and other deductions details
- Importing data into PowerBi
- As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential
###### Data Model
- Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor data modeling affects the overall performance of the report.
- Following Good practices of data modeling is must. Refer this page to get to know the good practices Blog
- In this project, we have followed Snowfall data modeling method.
![Data Model](https://github.com/user-attachments/assets/f163e6c3-19a0-4fb1-93ce-70de512e001a)
###### Dashboard designing
- Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required.
###### Home View
- In Home view, the entire views button will be available. User will land on specific view page by clicking the button
- Info
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Products
- Support
![HOME](https://github.com/user-attachments/assets/7687629d-ef62-4ed3-843b-3dc86032c15a)
###### Finance View
![FINANACE](https://github.com/user-attachments/assets/70680ea2-d00c-4ca6-8552-b8936a8fa124)
###### Sales View
![SALES](https://github.com/user-attachments/assets/c2cc20bb-a118-4d26-9e10-cdf6e66aa29e)
###### Marketing View
![MARKETING](https://github.com/user-attachments/assets/ac8907f6-ee12-4c6f-b496-183a64204b56)
###### Supply Chain View
![SC](https://github.com/user-attachments/assets/27e281be-4407-4627-8633-7c48c74dbdd3)
###### Executive View
![EXE](https://github.com/user-attachments/assets/8d8a8e56-fdd7-4fe0-ab8a-a3849a2421c3)
#### Project Outcome
- By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
#### You can find the full report file here :
(https://github.com/Vikas-engg1/Business-Insights-360/blob/main/New%20Buisness%20Insight%20360.pdf)_
