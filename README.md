# Northwind-Traders
### Maven Analytics
# Table of Contents
- Project Overview
- Data Sources
- Recommendations

# Project Overview
This project analyzes the sales performance of Northwind Traders, focusing on insights derived from sales data using SQL and Power BI. The analysis is designed to uncover key trends, highlight top-performing areas, and provide actionable insights for business decisions.

## Installation and Setup
1. Clone the repository:  
`git clone https://github.com/yaraazzam/Northwind-Traders-/`

2. Set up the required tools:
- Install SQL Server or your preferred SQL environment.
- Install Power BI Desktop.

3. Load the database and connect Power BI to perform analysis.

### Data Sources
https://mavenanalytics.io/data-playground

### Tools and Techniques
- SQL: For querying and cleaning the data.
[Download the Northwind Traders Sales Analysis](./QUERING_final.pdf)
 
- Power BI: For visualizing insights like top-selling products, sales by regions, and customer analysis.
  
###Data Cleaning/Preparation
In the initial data preparation phase, we performed the following tasks:

Data loading and inspection.
Handling missing values.
Data cleaning and formatting.
### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:
- What TOTAL SALES BY COUNTRY & CITY ?
- What TOP 5 CUSTOMERS ?
- What TOTAL AMOUNT SPENT BY EACH CUSTOMER ?
### Data Analysis
Include some interesting code/features worked with
```sql
SELECT 
	COUNT(*) AS TotalOrders
FROM orders;
```
## SQL Queries Example
Example query to fetch sales data:
```sql
SELECT ProductName, SUM(Quantity) as TotalSales
FROM Orders
GROUP BY ProductName
ORDER BY TotalSales DESC;
```

### Results/Findings
Total Revenue & Orders:
- Revenue: $1.35M
- Number of Orders: 830
- Best Performers:

- Top-Selling Product: Camembert Pierrot
- Top-Selling Categories:
- Condiments: $113,694.75
- Confections: $177,099.1
- Seafood: $141,623.09
- Top Employees:

- Highest Sales Contributors:
 Margaret Peacock
  Janet Leverling
Nancy Davolio
  Customer Insights:

- Top 5 Customers:
Horst Kloss: $117,483.39
Jose Pavarotti: $115,673.39
Patricia McKenna: $57,317.39
Detailed revenue distribution per customer highlights high-value targets.
Geographic Analysis:

- Top Countries:
USA
Germany
Austria
Sales heatmaps show regional performance, with USA leading in total revenue.
Sales Trends:
<img width="921" alt="Screenshot 2024-11-27 214806" src="https://github.com/user-attachments/assets/748ca11f-5a00-464e-8092-cdc017955394">

-Year-over-Year Sales Analysis (2013–2015):
Seasonal peaks identified, aiding in resource allocation and marketing efforts.
Monthly trends highlight key sales months.
<img width="915" alt="Screenshot 2024-11-27 214552" src="https://github.com/user-attachments/assets/99702efd-6fab-4ccf-b1d4-6307c51d4a2b">





# Recommendations
Present actionable takeaways based on your findings:

- Focus marketing on top customers (Horst Kloss, Jose Pavarotti).
- Invest in high-performing product categories (Confections, Seafood).
- Expand sales efforts in profitable regions (e.g., USA, Germany).

