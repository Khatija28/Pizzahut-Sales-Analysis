# Pizzahut-Sales-Analysis

Project Overview

The **Pizza Sales Analysis** project focuses on analyzing pizza sales data using SQL to understand business performance, customer ordering patterns, product preferences, and revenue trends.

The project uses a relational dataset containing information about pizza orders, pizza details, pizza categories, sizes, prices, and quantities.

Using **MySQL**, I performed data exploration and analysis by writing basic, intermediate, and advanced SQL queries. The analysis helps identify the most popular pizzas, highest revenue-generating products, customer ordering trends, and category-wise sales performance.

The project also demonstrates the practical application of SQL concepts in solving real-world business problems and extracting meaningful insights from structured data.

---


Project Objectives

- Analyze overall pizza sales and revenue performance.
- Identify the most popular pizza types and sizes.
- Understand customer ordering patterns.
- Analyze sales performance across different pizza categories.
- Identify peak ordering hours and daily sales trends.
- Calculate revenue contribution and cumulative revenue.
- Apply advanced SQL concepts to generate meaningful business insights.

---


Tools & Technologies Used

| Tool / Technology | Purpose |
|---|---|
| MySQL | Database management and SQL analysis |
| MySQL Workbench | Writing, executing, and managing SQL queries |
| SQL | Data retrieval, transformation, aggregation, and analysis |
| CSV Files | Source data used for importing records into MySQL |

---


Dataset Description

The project uses four CSV files, which were imported into MySQL to create a relational database.

1. Orders
Contains information about customer orders.

- `order_id` – Unique identifier for each order.
- `date` – Date on which the order was placed.
- `time` – Time at which the order was placed.

2. Order Details
Contains information about individual items included in each order.

- `order_details_id` – Unique identifier for each order detail.
- `order_id` – Reference to the corresponding order.
- `pizza_id` – Reference to the pizza ordered.
- `quantity` – Number of pizzas ordered.


3. Pizzas
Contains information about available pizzas.

- `pizza_id` – Unique identifier for each pizza variant.
- `pizza_type_id` – Reference to the pizza type.
- `size` – Pizza size.
- `price` – Price of the pizza.


4. Pizza Types
Contains information about pizza names, categories, and ingredients.

- `pizza_type_id` – Unique identifier for each pizza type.
- `name` – Name of the pizza.
- `category` – Pizza category.
- `ingredients` – Ingredients used in the pizza.


Database Relationships

The project uses the following relationships to combine information across tables:

- `orders` → `order_details` using `order_id`.
- `order_details` → `pizzas` using `pizza_id`.
- `pizzas` → `pizza_types` using `pizza_type_id`.

These relationships help retrieve information from multiple tables using SQL JOIN operations.

---


Project Workflow

1. **Dataset Collection:** Obtained the pizza sales dataset in CSV format.
2. **Database Creation:** Created a database in MySQL.
3. **Data Importing:** Imported the four CSV files into MySQL tables.
4. **Table Creation:** Created tables with appropriate column names and data types where required.
5. **Data Exploration:** Examined the tables, columns, records, and relationships.
6. **SQL Analysis:** Wrote and executed basic, intermediate, and advanced SQL queries.
7. **Result Analysis:** Interpreted query outputs to identify sales trends and business insights.
8. **Documentation:** Organized the SQL queries and their corresponding results for presentation.

---


Business Questions & SQL Analysis

The project addresses the following business questions to understand pizza sales performance.

1. Basic SQL Analysis

1. **How many total orders were placed?**
   - Retrieve the total number of unique orders.

2. **What is the total revenue generated from pizza sales?**
   - Calculate overall revenue using pizza prices and ordered quantities.

3. **Which pizza has the highest price?**
   - Identify the most expensive pizza available.

4. **Which order quantity occurs most frequently?**
   - Analyze the frequency of different ordered quantities.

5. **Which pizza size is ordered the most?**
   - Identify the most frequently ordered pizza size.

6. **What are the top 5 most ordered pizza types?**
   - Rank pizza types based on their total quantities sold.

2) Intermediate SQL Analysis

7. **What is the total quantity of pizzas ordered in each category?**
   - Calculate category-wise pizza sales quantities.

8. **How are orders distributed throughout the day?**
   - Analyze the number of orders placed during each hour.

9. **How many pizza types are available in each category?**
   - Determine the category-wise distribution of pizzas.

10. **What is the average number of pizzas ordered per day?**
    - Calculate the average daily pizza sales quantity.

11. **Which are the top 3 revenue-generating pizzas overall?**
    - Identify the pizzas contributing the highest revenue.

3. Advanced SQL Analysis

12. **What percentage of total revenue does each pizza type contribute?**
    - Calculate the percentage contribution of individual pizza types to overall revenue.

13. **What is the cumulative revenue generated over time?**
    - Calculate running revenue totals based on order dates.

14. **Which are the top 3 revenue-generating pizzas within each category?**
    - Rank pizzas based on revenue within their respective categories.

---


SQL Concepts & Techniques Applied

The project demonstrates the practical application of the following SQL concepts:

### Basic SQL Concepts
- SELECT and FROM statements
- WHERE clause
- ORDER BY
- GROUP BY
- LIMIT
- Aggregate Functions:
  - COUNT()
  - SUM()
  - AVG()
  - MAX()
- ROUND() function


Intermediate SQL Concepts
- INNER JOIN
- Joining multiple tables
- Table aliases
- GROUP BY with aggregate functions
- Sorting and filtering aggregated results
- Date and time functions
- Calculated columns and expressions


Advanced SQL Concepts
- Subqueries
- Window Functions
- RANK()
- OVER()
- PARTITION BY
- Running totals
- Percentage calculations
- Revenue contribution analysis
- Ranking products within categories

---


Key Areas of Analysis

The SQL queries focus on extracting insights from the following areas:

| Analysis Area | Business Purpose |
|---|---|
| Overall Sales | Understand total orders and revenue |
| Product Performance | Identify popular and high-value pizzas |
| Size Analysis | Understand customer size preferences |
| Category Analysis | Compare sales across pizza categories |
| Time-Based Analysis | Identify peak ordering hours and daily trends |
| Revenue Analysis | Evaluate revenue contribution and cumulative growth |
| Product Ranking | Identify top-performing pizzas overall and category-wise |

---


Repository Structure

```text
Pizza-Sales-Analysis-SQL/
│
├── README.md
│
├── Dataset/
│   ├── orders.csv
│   ├── order_details.csv
│   ├── pizzas.csv
│   └── pizza_types.csv
│
├── SQL_Queries/
│   ├── 01_Basic_Analysis.sql
│   ├── 02_Intermediate_Analysis.sql
│   └── 03_Advanced_Analysis.sql
│
├── Results/
│   └── Query_Results.pdf
│
└── Screenshots/
    └── SQL_Outputs/
```

---


Learning Outcomes

Through this project, I gained practical experience in:

- Working with relational databases using MySQL.
- Importing and managing CSV datasets.
- Understanding relationships between multiple database tables.
- Writing SQL queries to solve business-related problems.
- Applying JOIN operations to retrieve data from multiple tables.
- Using aggregate functions for sales calculations.
- Performing time-based and category-wise analysis.
- Applying subqueries and window functions for advanced analysis.
- Converting raw sales data into meaningful business insights.

---


 Conclusion

The Pizza Sales Analysis project demonstrates how SQL can be used to transform raw sales data into meaningful business information.

By applying basic, intermediate, and advanced SQL techniques, the project explores overall sales performance, product preferences, category-wise distribution, ordering patterns, and revenue trends.

This project strengthened my understanding of SQL and its application in data analysis, particularly in extracting insights that can support business decision-making.

---

**Project Domain:** Data Analytics  
**Project Type:** SQL Data Analysis  
**Database:** MySQL  
**Tool:** MySQL Workbench  

