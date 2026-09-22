### **E-Commerce Sales Dashboard**

##### 

##### 1\. Project Overview



The E-Commerce Sales Dashboard is an interactive Power BI project designed to analyze sales performance, profitability, product performance, customer segments, geographical distribution, and shipping patterns.



The dashboard provides a consolidated view of key business performance indicators and enables users to analyze sales trends across different categories, regions, products, and customer segments.



##### 2\. Business Objective



The main objectives of this project are to:



Monitor overall sales performance.



Track year-to-date sales, profit, and quantity.



Analyze profit margins.



Compare current performance with the previous year.



Identify top and bottom-performing products.



Analyze sales by category and region.



Understand geographical sales distribution.



Analyze sales based on shipping type.



Provide an interactive dashboard for business decision-making.





##### 3\. Tools \& Technologies



Power BI Desktop



Power Query



DAX



Microsoft Excel



Bing Maps





##### 4\. Dataset



The project uses an e-commerce sales dataset containing information related to:



Orders



Customers



Products



Categories



Sales



Profit



Quantity



Discounts



Order dates



Shipping dates



Shipping types



Customer regions



Customer states



Delivery status





##### 5\. Data Model



The Power BI model contains:



Fact Table



ecommerce\_data



Contains transactional sales information such as:



Order ID



Order Date



Product



Sales



Profit



Quantity



Discount



Customer information



Shipping information





Calendar Table



Calendar



Contains:



Date



Month



Month Number



Year





Supporting Table



us\_state\_long\_lat\_codes



Contains geographical information:



State



Name



Latitude



Longitude





The Calendar table is connected to the transaction table through the Order Date, while the geographical table supports state-level mapping.



##### 6\. Key KPIs



The dashboard includes:



YTD Sales



YTD Profit



YTD Quantity



YTD Profit Margin



PYTD Sales



PYTD Profit



PYTD Quantity



YoY Sales



YoY Profit



YoY Quantity



YoY Profit Margin





##### 7\. Dashboard Features



Sales by Category



Compares performance across:



Furniture



Office Supplies



Technology





The table includes YTD Sales, PYTD Sales, YoY Sales and trend indicators.



Top 5 Products



Identifies the five products with the highest YTD sales.



Bottom 5 Products



Identifies products with comparatively lower YTD sales.



Sales by State



Uses geographical visualization to display sales distribution across U.S. states.



YTD Sales by Region



Shows the contribution of different customer regions to overall YTD sales.



YTD Sales by Shipping Type



Shows sales distribution across different shipping methods.



Customer Segment



Allows analysis by:



Consumer



Corporate



Home Office





##### 8\. DAX \& Time Intelligence



DAX measures were created for year-to-date and previous-year analysis.



Example:



YTD Sales =

TOTALYTD(

&#x20;   SUM(ecommerce\_data\[sales\_per\_order]),

&#x20;   'Calendar'\[Date]

)



YTD profit margin is calculated using YTD profit divided by YTD sales:



YTD Profit Margin =

DIVIDE(

&#x20;   \[YTD Profit],

&#x20;   \[YTD Sales],

&#x20;   0

)

##### 

##### 9\. Dashboard Interactivity



The dashboard allows users to interact with the data through:



Customer segment selection



Category analysis



Regional analysis



Product analysis



Geographical filtering



Interactive Power BI visuals





##### 10\. Key Dashboard Results



At the displayed dashboard state, the dashboard reports approximately:



YTD Sales: $11.53M



YTD Profit: $1.34M



YTD Quantity: 107.2K



YTD Profit Margin: 11.58%





These values are dynamically calculated using Power BI measures.



##### 11\. Project Outcome



This project demonstrates the ability to:



Import and transform data.



Build a structured Power BI data model.



Create relationships between tables.



Develop DAX measures.



Apply time-intelligence calculations.



Design interactive dashboards.



Analyze business performance using visualizations.



Present data in a business-oriented format.







