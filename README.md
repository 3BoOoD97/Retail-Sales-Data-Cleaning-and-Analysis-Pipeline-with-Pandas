# Retail-Sales-Data-Cleaning-and-Analysis-Pipeline-with-Pandas


## Project Overview
This project analyzes a retail sales dataset to understand customer behavior, product performance, and sales trends. The goal is to clean the data, extract useful features, and generate insights that can help in making better business decisions.

- **What is the goal of the project?**  
  To explore and understand retail sales data by cleaning it, organizing it, and identifying meaningful patterns in customer behavior and sales.

- **What type of analysis was performed?**  
  Exploratory data analysis was performed, including checking data quality, analyzing sales over time, comparing product categories, and studying customer behavior based on gender and age groups.

- **Why is this project useful?**  
  It helps reveal how customers shop, which products perform best, and when sales are higher, supporting better business decisions.

---

##  Dataset Description
 This dataset is a snapshot of a fictional retail landscape, capturing essential attributes that drive retail operations and customer interactions. [View Dataset on Kaggle](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset)

- Number of rows: 1000
- Number of columns: 8
- Column names and their meaning:

### Columns:
- **Transaction ID**: A unique identifier for each transaction
- **Date**: The date when the transaction occurred
- **Customer ID**: A unique identifier for each customer  
- **Gender**: The gender of the customer (Male/Female)
- **Age**: The age of the customer  
- **Product Category**: The category of the purchased product  
- **Quantity**: The number of units of the product purchased 
- **Price per Unit**: The price of one unit of the product  
- **Total Amount**: The total monetary value of the transaction  

---

## Data Cleaning & Validation
I started by checking the overall quality of the data to make sure it is reliable for analysis.

- **Checked for missing values:** No missing values were found in the dataset.
- **Checked for duplicates:** Transaction IDs were unique, and there were no duplicate records.
- **Checked data types:** The data types were mostly correct, but the Date column was converted from string to datetime.
- **Validated consistency (Total Amount = Quantity × Price):**  All rows were consistent, and the total amount matched the expected calculation.
- **Checked for invalid or extreme values:** All numerical values (age, quantity, price, total amount) were within a reasonable range, with no negative or unrealistic values

### Findings:
No major issues were found in the dataset. The data was clean, with no missing values, duplicates, or inconsistencies.


---

##  Feature Engineering
To improve the analysis, I created a few new features from the existing data.

- **Converted Date to datetime:** This allows easier time-based analysis.
- **Extracted Month from Date:** This helps analyze sales trends over time.
- **Created Age Groups:** Ages were grouped into ranges to better understand customer behavior across different age segments.

### Why?
These features were created to make the data easier to analyze and more meaningful.  
Instead of working with raw values, they help reveal patterns, trends, and differences between customer groups more clearly.

---

## Analysis Performed

### 1️- Sales Over Time
- **What did I analyze?**
  I analyzed total sales for each month to understand how sales change over time.
- **What did I find?**
  Sales varied across months, with Month 5 having the highest sales and Month 4 the lowest. This suggests there may be seasonal patterns in customer purchases.

---

### 2️- Product Category Analysis
- **Which category performed best?**
  Electronics had the highest total sales, followed by Clothing, while Beauty had the lowest.
- **Observations?**
  The difference between Electronics and Clothing is small, which indicates strong demand for both categories, while Beauty is slightly behind.

---

### 3️- Gender Analysis
- **Who spends more?**
  Female customers spent more than male customers.
- **Is the difference significant?**
  The difference is small, so spending behavior is quite similar between genders.


---

### 4️- Age Group Analysis
- **Which age group spends the most?**
  The 36–50 age group generated the highest total sales, followed by the 50+ group.

- **Any patterns?**
  Spending tends to increase with age, which may be related to higher income.


---

### 5️-  Age Group vs Product Category
- **Do different age groups prefer different products?**
  Yes, different age groups show different preferences.
- **Key observations:**
  - Ages 50+ spend the most on Electronics  
  - Ages 36–50 prefer Beauty and also spend heavily on Electronics  
  - Ages 26–35 spend the most on Clothing  
  - Ages 18–25 spend more on Beauty

---

## Key Insights

- **Insight 1:** Sales vary across months, with a peak in Month 5 and a drop in Month 4, indicating possible seasonal patterns.
- **Insight 2:** Electronics and Clothing are the top-performing categories, showing strong and consistent demand compared to Beauty.
- **Insight 3:** Spending behavior is similar between genders, with females spending more but without a major difference.
- **Insight 4:** Older customers contribute the most to total sales, and each age group shows different product preferences.

---

## Conclusion

- The data shows that customer behavior varies based on age, product category, and time, with older customers contributing more to overall sales and different groups having different preferences.
- Overall, the dataset provides clear insights into sales trends and customer behavior, and even with simple analysis, we can identify useful patterns that could help in making better business decisions.

---

