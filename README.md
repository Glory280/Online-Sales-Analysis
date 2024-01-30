# Online Sales Analysis

## Table of Content
- [Project Overview](#project-overview)
- [About Data](#about-data)
- [Analysis List](#analysis-list)
- [Approached Used](#approached-used)
- [Insights and Recommendations](#insights-and-recommendations)


### Project Overview

This project involves conducting a comprehensive analysis for a UK-based online retail store to identify key factors influencing revenue. The management aims to strategically plan for the next year by examining metrics from both operations and marketing perspectives. Additionally, they seek insights into areas performing well to guide business expansion. The project's objectives include addressing operational and marketing questions, providing analytics for evaluating current performance, suggesting expansion metrics, and effectively communicating derived insights through advanced data analytics and visualization tools.

### About Data

The dataset was provided by TATA Group and it consists of 8 columns covering the following information;
- Invoice number
- Stock code
- Description of products
- Quantity ordered
- Invoice date
- Unit price
- Customer ID
- Country

### Analysis List

1 Sales Analysis
This analysis aims to answer the question of the sales of product in the past year. The result of this will provide imformation about the effectiveness of each sales strategy the business applies and what modificatoins are needed to gain more sales.

2 Customer Analysis
This analysis aims to uncover the different customers segments and purchase trends. The result will provide information about the top purchasing customers and how to retain them.

3 Country Analysis
This analysis aims to figure out the countries generating the most revenue and what strategies are needed to advance sales in those regions.

### Approached Used

1 Data Cleaning and Transformation: This is the first step where data is inspected to make sure NULL values and missing values are detected and data replacement methods are used to replace, missing or NULL values. The following tasks was performed;
- Data format: All columns consists of data of the correct format
- Missing values: I filtered, checked and got rid of any available missing values.
- Duplicate values: I ensured all the rows and columns were unique and free from
duplicate values.
- Data extraction: For clearer analysis, I extracted the month and day of the week from the
order date column using the “create column feature”
- Incorrect values: For better analysis, I got rid of values not accurate for analysis like price
values below “$0” and quantity values below “1” using DAX formulas and conditional
formatting.

2 Exploratory Data Analysis and Visualization: This is done to answer key questions such as;
- Which region is generating the highest revenue, and which region is generating the lowest?
- What is the monthly trend of revenue, which months have faced the biggest increase/decrease?
- Which months generated the most revenue? Is there a seasonality in sales?
- Who are the top customers and how much do they contribute to the total revenue? 
- What day of the week generates the most sales?
- What are the top 5 revenue generating products?


### Insights and Recommendations
- In the year 2011, the online retail store generated a total of $8,000,000 revenue and a total of 4.9 million total purchases were made.
- My analysis shows that there are some months of the year where exceptional growth is witnessed. The data shows that the revenue in the first 8 months is fairly constant as the average revenue generated for these 8 months is around $685k. The increase in revenue starts in the month of September, where the revenue increases by 40% over the previous month. This trend continues till the month of November where it reached 1.5 million USD, the highest during the entire year. The data is incomplete for the month of December, therefore, no conclusion can be drawn from it, unfortunately. This analysis shows that the retail store sales are impacted by the seasonality which usually occurs in the last 4 months of the year.
- Countries such as the Netherlands, Ireland, Germany and France have high volumes of units bought and revenue generated (This does not include the UK as the country already has high demand and I was told to focus only on the countries where demand can be increased). I would suggest that these countries should be focused on to ensure that measures are taken to capture these markets even more.
- There is not much of a difference between the purchases made by the top 10 customers. The highest revenue generating customer only purchased 17% more than the 2nd highest which shows that the business is not relying only on a few customers to generate the revenue. This shows that the bargaining power of customers is low and the business is in a good position.
- White hanging heart T-light holder, Jumbo bag red retrospot, Assorted color bird ornament, Pack of 72 retrospot cake cases and World war 2 glider assorted designs were the top 5 products of the year. I would suggest the customers are educated on the best selling products. This will increase their confidence and trust in the retailer thereby making more purchases and increasing sales.
- [View Dashboard](https://drive.google.com/file/d/1dqVtLnogzFCc7CznkYJPaSeViqcXh5zG/view?usp=sharing)

### DAX Calculation
1 Revenue
 Revenue=
 Quantity*UnitPrice
