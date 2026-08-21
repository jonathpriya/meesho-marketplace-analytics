# Meesho Marketplace Analytics and Business Intelligence Dashboard

## Project Overview

The **Meesho Marketplace Analytics and Business Intelligence Dashboard** is an end-to-end Business Intelligence and Data Analytics project developed to analyse Meesho marketplace data using **MySQL and Microsoft Power BI**.

The project focuses on analysing key marketplace activities such as orders, products, customers, sellers, deliveries and returns. MySQL is used for database management and SQL-based analysis, while Power BI is used to transform the data into interactive dashboards and meaningful business insights.

The dashboard helps understand marketplace performance, identify trends, analyse customer and seller behaviour, evaluate product and order performance, and monitor return and delivery-related metrics.

---

## Project Objectives

- Analyse overall marketplace performance.
- Analyse order, product, customer, seller, delivery and return data.
- Identify high-performing and low-performing products.
- Analyse customer purchasing and return behaviour.
- Evaluate seller performance.
- Analyse delivery performance and order status.
- Identify return trends and patterns.
- Create meaningful KPIs using DAX.
- Develop interactive Power BI dashboards.
- Generate data-driven business insights to support decision-making.

---

## Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| **MySQL** | Database creation, storage and SQL analysis |
| **MySQL Workbench** | Database management and query execution |
| **Microsoft Power BI** | Interactive dashboards and data visualization |
| **DAX** | KPI and calculated measure creation |
| **Power Query / ETL** | Data transformation and preparation |
| **Excel / CSV** | Dataset preparation and source data |
| **GitHub** | Project documentation and version control |

---

## Dataset Description

The dataset contains marketplace-related information covering different aspects of an e-commerce platform.

### Main Tables

- **Customers** – Customer information and customer-related attributes.
- **Products** – Product details and product categories.
- **Sellers** – Seller information and seller-related attributes.
- **Orders** – Order and transaction information.
- **Delivery** – Delivery and order delivery details.
- **Returns** – Returned order/product information.

The dataset was imported into MySQL, where the tables were organized into a relational database for further analysis.

---

## SQL Analysis

SQL was used to explore, analyse and extract meaningful information from the marketplace database.

The analysis includes:

- Database and table creation.
- Data exploration and validation.
- Filtering and sorting data.
- Aggregation using `COUNT()`, `SUM()`, `AVG()`, `MIN()` and `MAX()`.
- `GROUP BY` and `ORDER BY` analysis.
- Joins between multiple tables.
- Customer-level analysis.
- Product-level analysis.
- Seller-level analysis.
- Order analysis.
- Return analysis.
- Delivery performance analysis.
- Identification of high-return and high-performing products.

The complete database has been exported as a `.sql` file and is included in the repository.

---

## Power BI Dashboard

Microsoft Power BI was used to build an interactive Business Intelligence dashboard from the MySQL database.

The dashboard provides analysis of:

- Overall marketplace performance.
- Order performance.
- Product performance.
- Customer behaviour.
- Seller performance.
- Delivery performance.
- Return performance.
- Category-wise trends.
- Order and return trends.

The dashboard contains interactive KPI cards, charts, filters and slicers that allow users to explore marketplace data from different perspectives.

---

# Dashboard Pages

## Page 1 – Executive Dashboard

### Purpose

Provides a high-level overview of overall marketplace performance.

### Key Analysis

- Total Orders
- Total Sales
- Total Returns
- Return Rate
- Total Refund
- Average Order Value
- Delayed Orders
- Delay Rate
- Monthly Sales & Returns Trend
- Return by Reason
- Delivery Performance
- Orders by Payment Method
- Top 10 Returned Products
- Top 10 Sellers by Returns
- Category-wise Return Rate
- Refund by Category

---

## Page 2 – Return Intelligence

### Purpose

Focuses on return behaviour, refund impact and customer risk analysis.

### Key Analysis

- Total Refund
- Average Refund
- Total Returns
- Return Rate
- Monthly Returns Trend
- Return by Reason
- Monthly Refund Trend
- Category-wise Return Rate
- Top 10 Products by Return Rate
- Refund by Category
- Top 10 High-Risk Customers
- Customer Fraud Risk Distribution

---

## Page 3 – Performance & Risk Score

### Purpose

Focuses on seller performance, seller risk and delivery risk.

### Key Analysis

- Seller Performance Score
- High-Risk Seller
- Average Seller Score
- Seller Risk Rate
- Top 10 Sellers by Performance Score
- Top 10 Risk Sellers by Return Rate
- Seller Performance vs Return Rate
- State-wise Seller Performance
- State-wise Delivery Risk
- Seller Performance Distribution
- Seller Risk Category
- High-Risk Seller by State

---

## Key KPIs

The dashboard includes important business KPIs such as:

| KPI | Description |
|---|---|
| **Total Orders** | Total number of orders |
| **Total Returns** | Total number of returned orders/products |
| **Return Rate** | Percentage of orders that were returned |
| **Total Customers** | Total number of customers |
| **Total Products** | Total number of products |
| **Total Sellers** | Total number of sellers |
| **Average Order Value** | Average value of orders |
| **Delivery Performance** | Analysis of delivery-related performance |

KPI values are calculated dynamically in Power BI using DAX measures.

---

## Customer Risk Analysis

Customer risk analysis is included in the **Return Intelligence** page.

The risk analysis uses return-related behaviour such as:

- Return Rate
- COD Returns
- Damaged Returns
- Refund behaviour

### Risk Score

```text
Risk Score =
(Return Rate × 50)
+ (COD Returns × 5)
+ (Damaged Returns × 5)
```

The score is limited to a maximum of 100.

### Risk Level

| Risk Score | Risk Level |
|---:|---|
| 70 and above | High Risk |
| 40–69 | Medium Risk |
| Below 40 | Low Risk |

The risk analysis is rule-based and is intended to identify potentially suspicious behaviour patterns. A high-risk score does not prove that a customer has committed fraud.

---

## Key Insights

The analysis helps identify important business insights such as:

- Products and categories with high order volumes.
- Products and categories contributing to higher returns.
- Customer purchasing and return patterns.
- Seller-wise performance and return behaviour.
- Delivery performance and its relationship with orders.
- Product categories requiring further attention.
- Overall order and return trends.
- Marketplace areas that can be improved through data-driven decisions.

These insights can help improve marketplace performance, customer satisfaction, seller performance, delivery efficiency and return management.

---

## Project Workflow

```text
Dataset
   ↓
Data Collection & Preparation
   ↓
Data Cleaning
   ↓
MySQL Database Creation
   ↓
Table Import
   ↓
SQL Analysis
   ↓
Connect MySQL with Power BI
   ↓
Power Query / ETL
   ↓
Data Transformation
   ↓
DAX Measures & KPIs
   ↓
Dashboard Design
   ↓
Filters & Slicers
   ↓
Business Insights
```

---

## Filters & Slicers

The dashboard includes interactive filters and slicers for data exploration.

### Main Filters

- Date Range
- State
- Category
- Payment Method

### Navigation

Users can navigate between:

- Executive Dashboard
- Return Intelligence
- Performance & Risk Score

The dashboard also supports interactive visual filtering and cross-filtering.

---

## Repository Structure

```text
Meesho-Marketplace-Analytics/
│
├── README.md
│
├── Database/
│   └── meesho_marketplace.sql
│
├── PowerBI/
│   └── Meesho_Project.pbix
│
├── SQL/
│   └── SQL_Analysis_Queries.sql
│
├── Dataset/
│   └── Dataset.csv
│
├── Screenshots/
│   ├── Dashboard_Overview.png
│   ├── Return_Intelligence.png
│   └── Performance_Risk_Score.png
│
└── Documentation/
    └── Project_Documentation.pdf
```

> Update the filenames in this structure if your uploaded repository filenames are different.

---

## Dashboard Screenshots

### Executive Dashboard

Place the screenshot at:

```text
Screenshots/Dashboard_Overview.png
```

### Return Intelligence

Place the screenshot at:

```text
Screenshots/Return_Intelligence.png
```

### Performance & Risk Score

Place the screenshot at:

```text
Screenshots/Performance_Risk_Score.png
```

---

## How to Run the Project

### Prerequisites

- MySQL Server
- MySQL Workbench
- Microsoft Power BI Desktop

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

### 2. Set Up the MySQL Database

1. Open MySQL Workbench.
2. Connect to your MySQL Server.
3. Open:

```text
Database/meesho_marketplace.sql
```

4. Execute the complete SQL script.
5. Verify that the `meesho_project` database and required tables are available.

The SQL script contains the exported database structure and data.

### 3. Run SQL Analysis

If the SQL analysis file is included, open:

```text
SQL/SQL_Analysis_Queries.sql
```

Execute the required queries in MySQL Workbench.

### 4. Open Power BI

Open the Power BI project file:

```text
PowerBI/Meesho_Project.pbix
```

### 5. Connect Power BI to MySQL

If Power BI asks for database credentials:

1. Select **MySQL Database**.
2. Enter the MySQL Server details.
3. Select the `meesho_project` database.
4. Enter the required MySQL credentials.
5. Refresh the dataset.

### 6. Explore the Dashboard

Use the available filters, slicers, KPI cards and visualizations to interact with the dashboard and analyse marketplace performance.

---

## Project Limitations

- Customer risk analysis is rule-based.
- The risk score depends on the selected business rules and available indicators.
- A high-risk score indicates potentially suspicious behaviour and does not prove fraud.
- Dashboard analysis depends on the quality and completeness of the source dataset.
- The project is designed as an analytics dashboard using the available project data.

---

## Future Enhancements

Possible future enhancements include:

- Advanced fraud detection techniques.
- Additional customer behaviour indicators.
- Automated alerts for unusual return/refund patterns.
- Advanced seller analysis.
- Advanced customer segmentation.
- Predictive analysis for future returns.

These are future possibilities and are not part of the current implementation.

---

## Conclusion

The **Meesho Marketplace Analytics and Business Intelligence Dashboard** demonstrates an end-to-end analytics workflow using MySQL and Power BI.

The project transforms marketplace data into meaningful business insights by combining SQL analysis, ETL, DAX calculations and interactive Power BI visualizations.

It provides a comprehensive view of products, customers, sellers, orders, deliveries and returns to support data-driven business decisions.

---

## Author

**Dharshini Priya**

**B.Tech – Artificial Intelligence and Data Science**

### Skills Used

- MySQL
- SQL
- Power BI
- DAX
- Power Query
- ETL
- Data Cleaning
- Data Visualization
- Business Intelligence
- Data Analytics
