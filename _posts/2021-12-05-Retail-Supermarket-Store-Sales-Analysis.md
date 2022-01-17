---
title: Retail Supermarket Store Sales Analysis
date: 2021-12-05 13:45:00 +0530 
tags: [Machine learning, R, Exploratory Data Analysis, Regression]
comments: false
img_path: /assets/img/2021-12-05-Retail-Supermarket-Store-Sales-Analysis
---

###  Summary
This is an academic project completed by me as part of my Post Graduate program in Data Science from Purdue University through Simplilearn. The project was towards the completion of Data Science with R module. 

You can view the full project code on this [Github link](https://github.com/Ransomk/Retail-Supermarket-Store-Sales-Analysis)

The project includes an analysis of a Giant retail supermarket chain's sales data for a period of 2.5 years using R to build a model for forecasting Sales and demand.
The project also includes exploratory analysis of the store data to review the effect of markdowns due to holidays on the sales. Do the markdowns and discounts help sales during the holiday season. Along with this there was also general insights about the sales across the various locations/outlets to identify stores with most sales and variation in sales across stores and across months etc.

### Bussiness Scenario
One of the leading retail stores in the US, Walmart, would like to predict the sales and demand accurately. There are certain events and holidays which impact sales on each day. There are sales data available for 45 stores of Walmart. The business is facing a challenge due to unforeseen demands and runs out of stock some times, due to the inappropriate machine learning algorithm. An ideal ML algorithm will predict demand accurately and ingest factors like economic conditions including CPI, Unemployment Index, etc.
Walmart runs several promotional markdown events throughout the year. These markdowns precede prominent holidays, the four largest of all, which are the Super Bowl, Labour Day, Thanksgiving, and Christmas. The weeks including these holidays are weighted five times higher in the evaluation than non-holiday weeks. Part of the challenge presented by this competition is modeling the effects of markdowns on these holiday weeks in the absence of complete/ideal historical data. Historical sales data for 45 Walmart stores located in different regions are available.

### Analysis Steps

1. Answer questions based on Exploratory Data Analysis like: 
 - Find the store which has maximum sales and store with maximum standard deviation i.e., the sales vary a lot. 
 - Which store/s has good quarterly growth rate in Q3’2012
 - Some holidays have a negative impact on sales. Find out holidays which have higher sales than the mean sales in non-holiday season for all stores together
2. Creating a monthly and semester view of sales in units and insights on the same.
3. Building prediction models to forecast demand based on the data features.
4. Linear Regression models built and analysed for features leading to best possible accuracy.
5. Hypothesize if CPI, unemployment, and fuel price have any impact on sales.
6. Conclusions and select the model which gives best accuracy.

### Insights and conclusion
Here are a few insights based on the project:
1. Based on the analysis and models built for Store #1 we see that none of the variables in the data captured reflect as accurate predictors of Sales/Demand.
2. Suggest to build and test models for other stores randomly to again verify if there is no strong predictors for Sales. As the analysis of sales data store by store revealed that the stores have some differences in terms of average sales volume as well as Variability of sales. Also stores located in different regions are not always fully homogeneous.
3. We also see that month appears to impact the sales quite well as there were some trends seen in the month- wise sales analysis.

![Monthwise_sales](11-Monthly-Average-Sales.png){: w="360" .left} 
![Boxplot_monthly_sales](12-Box-Plot-Monthly-Sales-Analysis.png){: w="360" .right}
![Semester_sales](15-Semester-Average-Sales.png){: w="360" .left} 
![Boxplot_semesterwise_sales](16-Box-Plot-Semester-Sales-Analysis.png){: w="360" .right}

4. The hypothesis tested for CPI, Unemployment and Fuel price revealed again that which economic factors like CPI and unemployment do show some impact on sales. They cannot accurately help predict the sales.
![Correlation_pairplot](28-Plot-Weekly-Sales-vs-other-variables.png)

5. Holiday v/s non-holiday sales comparison showed that for most Holidays except Christmas the Average Sales are higher. While this was a good study if the overall revenue was under consideration. As suggested this comparison is limited when trying to analyse units sold due to the fact that the prices of goods during the holidays. Since the date available is only in amount sold in dollar value. This doesn’t help identify the increase in number of units of stock/goods that were sold due to the discounts provided in the Holidays. So from an inventory perspective to predict the number of units which Walmart would need to keep in stock this does not help provide any clear insight. Although this could be assessed if the discount rates were known for various categories.
6. Finally to conclude. For Walmart to better predict the sales/demand and create a model to predict the inventory requirements to prevent stockouts. The model would need to consider or incorporate other variables which may have more significant impact on sales. These could be for example. Season of the year, Median neighbourhood incomes, Inflation rates etc. which could affect sales of some or many products. Also analysis of products based on categories is recommended as not all products in a supermarket have the same sales/demand requirements all throughout the year.
Walmart could try to focus on specific major product categories and then try to see if they can create more accurate predictions for the demand for the categories alone. This could help in ensuring that demand for such products can be predicted well and stock can be maintained according to the anticipated demand.


### Tools used:
This project was completed in R programming lanuage and 
used various statistical packages within R like dplyr, lubridate, sp, raster, usdm
