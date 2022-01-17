---
title: Retail Supermarket Store Sales Analysis
date: 2021-12-05 13:45:00 +0530 
tags: [Machine learning, R, Exploratory Data Analysis, Linear Regression]
comments: false
img_path: /assets/img/2021-12-05-Retail-Supermarket-Store-Sales-Analysis
---

### Summary-

The project includes an analysis of a Giant retail supermarket chain's sales data for a period of 2.5 years using R to build a model for forecasting Sales and demand.  
The project also includes exploratory analysis of the store data to review the effect of markdowns due to holidays on the sales. Do the markdowns and discounts help sales during the holiday season. Along with this there was also general insights about the sales across the various locations/outlets to identify stores with most sales and variation in sales across stores and across months etc.

You can view the full project code on this [Github link](https://github.com/Ransomk/Retail-Supermarket-Store-Sales-Analysis)

Note: _This is an academic project completed by me as part of my Post Graduate program in Data Science from Purdue University through Simplilearn. The project was towards the completion of Data Science with R module._

### Bussiness Scenario
One of the leading retail stores in the US, Walmart, would like to predict the sales and demand accurately. There are certain events and holidays which impact sales on each day. There are sales data available for 45 stores of Walmart. The business is facing a challenge due to unforeseen demands and runs out of stock some times, due to the inappropriate machine learning algorithm. An ideal ML algorithm will predict demand accurately and ingest factors like economic conditions including CPI, Unemployment Index, etc.
Walmart runs several promotional markdown events throughout the year. These markdowns precede prominent holidays, the four largest of all, which are the Super Bowl, Labour Day, Thanksgiving, and Christmas. The weeks including these holidays are weighted five times higher in the evaluation than non-holiday weeks. Part of the challenge is modeling the effects of markdowns on these holiday weeks in the absence of complete/ideal historical data. Historical sales data for 45 Walmart stores located in different regions are available.

### Analysis Steps

1. Answer few questions based on Exploratory Data Analysis like: 
 - Find the store which has maximum sales and store with maximum standard deviation i.e., the sales vary a lot. 
 - Which store/s has good quarterly growth rate in Q3’2012
 - Some holidays have a negative impact on sales. Find out holidays which have higher sales than the mean sales in non-holiday season for all stores together
2. Creating a monthly and semester view of sales in units and insights on the same.  
    ![Monthwise_sales](11-Monthly-Average-Sales.png){: w="340"} 
    ![Boxplot_monthly_sales](12-Box-Plot-Monthly-Sales-Analysis.png){: w="340"} 
    ![Semester_sales](15-Semester-Average-Sales.png){: w="340"} 
    ![Boxplot_semesterwise_sales](16-Box-Plot-Semester-Sales-Analysis.png){: w="340"}
3. Building prediction models to forecast demand based on the data features.
4. Linear Regression models built and analysed for features leading to best possible accuracy.
5. Hypothesize if CPI, unemployment, and fuel price have any impact on sales.
    ![Correlation_pairplot](28-Plot-Weekly-Sales-vs-other-variables.png){: w="700" .normal} 
6. Conclusions and select the model which gives best accuracy.


### Tools used:
This project was completed in R programming lanuage and 
used various statistical packages within R like dplyr, lubridate, sp, raster, usdm
