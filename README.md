Overview:
This project analyzes customer shopping behaviour using transactional purchase data. The goal is to understand how customers shop, how much they spend, and which factors influence purchasing decisions such as discounts, subscriptions, and demographics.
The project follows a complete data analytics workflow, including data loading, cleaning, exploratory data analysis (EDA), SQL-based business analysis, and dashboard visualization. Insights are summarized through a Power BI dashboard, a written report, and a presentation created using Gamma.

Dataset:
The dataset used in this project contains 3,900 purchase records and 18 columns describing customer demographics, purchase details, and shopping behaviour.
Key data fields include:
Customer Information-
Age
Gender
Location
Subscription Status

Purchase Details-
Item Purchased
Category
Purchase Amount
Season
Size
Colour

Shopping Behaviour-
Discount Applied
Promo Code Used
Previous Purchases
Frequency of Purchases
Review Rating
Shipping Type

During data exploration, 37 missing values were identified in the Review Rating column, which were handled during the data cleaning process.

Tools and Technologies:
Python – Data loading, cleaning, and exploratory analysis
Pandas – Data manipulation and preprocessing
PostgreSQL – Writing analytical SQL queries
Power BI – Interactive dashboard creation
Gamma – Presentation design
Jupyter Notebook – Analysis workflow and documentation

Project Steps:
1. Data Loading
The dataset was imported into Python using the Pandas library and loaded into a DataFrame for analysis.

2. Data Cleaning
Several preprocessing steps were performed:
Missing values in the Review Rating column were replaced with the median rating of each product category.
Column names were standardized into snake_case format.
Data consistency checks were performed.
The promo_code_used column was removed because it contained information similar to discount_applied.

3. Feature Engineering
New variables were created to improve analysis:
age_group – Groups customers into age ranges.
purchase_frequency_days – Helps analyze how frequently customers make purchases.

4. Database Integration
The cleaned dataset was uploaded to a PostgreSQL database, allowing further analysis through SQL queries.

5. SQL Analysis
Several business questions were answered using SQL, including:
Revenue comparison by gender
Identification of high-spending customers using discounts
Top 5 products with the highest average ratings
Comparison of spending by shipping type
Subscriber vs non-subscriber spending behaviour
Products most dependent on discounts
Customer segmentation (new, returning, loyal)
Top 3 most purchased products per category
Relationship between repeat purchases and subscriptions
Revenue contribution by age group

Dashboard:
A Power BI dashboard was built to visualize key insights from the analysis.
The dashboard highlights:
Customer demographics
Product performance
Revenue trends
Discount usage
Customer shopping patterns
Interactive visualizations help stakeholders quickly understand trends and patterns in the data.

Key Results:
The analysis produced several insights, including:
Certain product categories generate significantly higher revenue.
Customers who frequently purchase are more likely to subscribe.
Some products rely heavily on discounts to drive purchases.
Specific age groups contribute more to overall sales.
Highly rated products tend to have stronger demand.
These insights can support better marketing strategies, pricing decisions, and customer engagement initiatives.
