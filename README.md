# Company-Sales-Analysis
Sales Aanalysis

## Table of Contents

- [Project Overview](#project-overview)

- [Data Source](#data-source)

- [Tools](#tools)

- [Data Cleaning/Preparation](#data-cleaningpreparation)

- [Exploratory Data Analysis](#exploratory-data-analysis)

- [Results / Findings](#resultsfindings)

- [Recommendations](#recommendations)

- [Limitations](#limitations)

- [References](#references)

### Project Overview

This is a python and SQL project on an imaginary supermarket called Nasa Supermarket. the analysis project objectives is to analyze and glean insight into the sales performance of Nasa Supermarket for the year 2023. By analyzing various aspect of the sales data, we want to identify trends, make data-driven recommendations, and gain a deeper understanding of the supermarket’s (company) performance to answer critical questions and help the supermarket make data-driven decisions.


![sales1](https://github.com/CChukwu-data-analyst/Company-Sales-Analysis/assets/170612341/82a73934-6e58-424b-8b09-7918e6a182e6)

### Data Source

Sales data: The primary dataset used for this analysis is the “Sales_data.csv” file, containing detail information about each sale made by the supermarket for the period under review.

### Tools

- Python Pandas - Data Reading
- Python Matplotlib - Data Visualization 
- SQL Server
   - [Download here](https://enhtechsoftware.com)
- PowerBI - Creating Reporting

### Data Cleaning/Preparation

  In the initial data preparation phase, I performed the following tasks:

  1.	Data loading and Inspection
  2.	Handling missing values
  3.	Data cleaning and formatting

### Exploratory Data Analysis

EDA involves exploring the sales data to answer important business questions such as:

-	What is the overall sales trend?
-	Which products are top sellers? 
-	What are the peak sales period?

### Data Analysis

Some interesting codes/ features worked with 

```python
sales_df = pd.read_csv("C:/Users/Nasa/Databank Analysis/Dataframes/sales.csv")
```
```python
sales_df.columns = [i.lower() for i in sales_df.columns]
```
```sql
get_sales = 'select * from sales'
sales_df = pd.read_sql(get_sales, conn)
```

### Results/Findings

The following are the summary of the analysis:

1.	The supermarket sales has been steadily increasing over the past year, with a noticeable peak during the holiday seasons
2.	Product category cloths, sockets, and Phones are the best performing category in terms of sales and revenue generation
3.	Customer segment with high live time value (LTV) should be targeted for marketing efforts

### Recommendations

Based on the just concluded analysis, we here by recommended the following actions:

-	Invest in marketing and promotions during peak sales seasons to maximize revenue
-	Focus on expanding and promoting products categories cloths, sockets, and phones
-	Implement a customer segmentation strategy to target high LTV customers effectively

### Limitations

I have to remove all missing values and zeros from Tuesday to Friday columns because they would have impacted the accuracy of my result or conclusion from the analysis. There are still a few outliers even after the verifications but even then, we can still see that there is a positive correlation between daily sales and products.

### References

1. SQL for beginners
2. Stack Overflow

😄
