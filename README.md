# Walmart Sales Data Analysis

This project analyzes Walmart sales data to gain insights into the company's highest-performing stores and products, sales trends across different product categories, and customer purchasing behavior. The goal is identifying opportunities to enhance and optimize Walmart's sales strategies. The raw data was sourced from a Kaggle competition focused on forecasting Walmart sales. By studying historical sales patterns across Walmart's branches, products, and customer segments, this project aims to uncover actionable ways the retail giant can boost revenues in the future. 


**Purposes Of The Project**
The major aim of the project is to gain insight into the sales data of Walmart to understand the different factors that affect sales of the different branches.

**About Data**
The dataset was obtained from the Kaggle Walmart Sales Forecasting Competition. This dataset contains sales transactions from three different branches of Walmart, located in Mandalay, Yangon, and Naypyitaw. The data contains 17 columns and 1000 rows:
https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting

**Column	Description	Data Type**
| Column | Description | Data Type |
|-|-|-|  
| invoice_id | Invoice of sales made | VARCHAR(30) |
| branch | Branch at which sales were made | VARCHAR(5) |
| city | The location of the branch | VARCHAR(30) |
| customer_type | The type of the customer | VARCHAR(30) |
| gender | Gender of the customer making purchase | VARCHAR(10) |
| product_line | Product line of the product solf | VARCHAR(100) |
| unit_price | The price of each product | DECIMAL(10, 2) |
| quantity | The amount of the product sold | INT |
| VAT | The amount of tax on the purchase | DECIMAL(6, 4) |
| total | The total cost of the purchase | DECIMAL(10, 2) |
| date | The date on which the purchase was made | DATE |
| time | The time at which the purchase was made | TIMESTAMP | 
| payment_method | The total amount paid | DECIMAL(10, 2) |
| cogs | Cost Of Goods sold | DECIMAL(10, 2) |
| gross_margin_percentage | Gross margin percentage | DECIMAL(11, 9) |
| gross_income | Gross Income | DECIMAL(10, 2) |
| rating | Rating | DECIMAL(2, 1) |

# Analysis List

**Product Analysis**
This project will analyze Walmart's product data to identify top-selling items, underperforming product lines, and opportunities to optimize the company's merchandise mix. The goal is to understand which products drive the most sales and profits for Walmart so they can double down on winning categories while reevaluating slower-moving items.

**Sales Analysis**
By examining historical sales data across products, stores, seasons, and customer demographics, this analysis aims to uncover sales trends and patterns. The findings will be used to measure the effectiveness of current sales strategies and determine where changes may be needed to improve revenues. Sales analysis provides actionable insights to boost performance.

**Customer Analysis**
This portion of the project will focus on segmenting Walmart shoppers based on their purchase behaviors over time. The goal is to identify the most valuable customer groups, trends, and profitability levels. These customer insights can inform marketing and merchandising decisions to optimize satisfaction and loyalty across segments.

---Approach Used
Here is GitHub markdown to format the content aesthetically:

# Approach Used

1. **Data Wrangling:** This is the first step where inspection of data is done to make sure **NULL** values and missing values are detected and data replacement methods are used to replace, missing or **NULL** values.

    - Build a database
    
    - Create table and insert the data.
    
    - Select columns with null values in them. There are no null values in our database as in creating the tables, we set **NOT NULL** for each field, hence null values are filtered out.
    
2. **Feature Engineering:** This will help use generate some new columns from existing ones.

    - Add a new column named `time_of_day` to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.
    
    - Add a new column named `day_name` that contains the extracted days of the week on which the given transaction took place (Mon, Tue, Wed, Thur, Fri). This will help answer the question on which week of the day each branch is busiest.
    
    - Add a new column named `month_name` that contains the extracted months of the year on which the given transaction took place (Jan, Feb, Mar). Help determine which month of the year has the most sales and profit.
    
3. **Exploratory Data Analysis (EDA):** Exploratory data analysis is done to answer the listed questions and aims of this project.

4. **Conclusion:**

# Business Questions To Answer

## Generic Question

1. How many unique cities does the data have?

2. In which city is each branch?

## Product 

1. How many unique product lines does the data have?

2. What is the most common payment method? 

3. What is the most selling product line?

4. What is the total revenue by month?

5. What month had the largest COGS? 

6. What product line had the largest revenue?

7. What is the city with the largest revenue? 

8. What product line had the largest VAT?

9. Fetch each product line and add a column to those product line showing "Good", "Bad". Good if its greater than average sales  

10. Which branch sold more products than average product sold?

11. What is the most common product line by gender?

12. What is the average rating of each product line?

## Sales

1. Number of sales made in each time of the day per weekday

2. Which of the customer types brings the most revenue?

3. Which city has the largest tax percent/ VAT (**Value Added Tax**)?

4. Which customer type pays the most in VAT?

## Customer

1. How many unique customer types does the data have?

2. How many unique payment methods does the data have?

3. What is the most common customer type? 

4. Which customer type buys the most?

5. What is the gender of most of the customers?

6. What is the gender distribution per branch? 

7. Which time of the day do customers give most ratings?

8. Which time of the day do customers give most ratings per branch?

9. Which day fo the week has the best avg ratings?

10. Which day of the week has the best average ratings per branch?
