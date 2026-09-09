# AdventureWorks Sales & Customer Analytics Dashboard

An interactive Power BI dashboard built using the AdventureWorks dataset to analyze sales performance, profitability, orders, returns, products, customers, and geographic performance.

## Dashboard Overview

The dashboard provides a multi-page analytical view of business performance, allowing users to move from high-level KPIs to product-, customer-, and regional-level insights.

### Key Metrics

- Total Revenue
- Total Profit
- Total Orders
- Return Rate
- Total Customers
- Revenue per Customer
- Monthly Revenue
- Monthly Orders
- Monthly Returns

---

## Data Model

The Power BI report uses a relational analytical data model consisting of transactional fact tables and lookup/dimension tables.

### Main Tables

#### Fact Tables

- **Sales Data** – Contains transactional sales information including customer, product, territory, order date, order quantity, and order details.
- **Returns Data** – Contains product return information including return date, product, return quantity, and territory.

#### Lookup / Dimension Tables

- **Calendar Lookup** – Provides date attributes such as month, quarter, week, and year.
- **Customer Lookup** – Contains customer information and demographic attributes such as income level, education, occupation, and other customer characteristics.
- **Product Lookup** – Contains product information including product name, pricing, cost, SKU, product description, and product characteristics.
- **Territory Lookup** – Contains geographic attributes including continent, country, region, and sales territory.
- **Product Subcategories** – Provides product subcategory information.
- **Product Categories** – Provides the higher-level product category structure.

### Model Structure

The model connects transactional sales and returns data to reusable lookup tables, allowing consistent analysis across multiple business dimensions.

Key relationships include:

- Calendar → Sales
- Calendar → Returns
- Customer → Sales
- Product → Sales
- Product → Returns
- Territory → Sales
- Territory → Returns
- Product → Product Subcategories → Product Categories

The product hierarchy is structured as:

**Product → Product Subcategory → Product Category**

This model supports analysis across time, customers, products, territories, categories, and returns.

![AdventureWorks Data Model](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20134854.png?raw=true)

---

## Dashboard Pages

### 1. Sales Overview

The sales overview page provides a high-level view of overall business performance.

Key components:

- Revenue trend
- Orders by category
- Top 10 products
- Product revenue
- Return contribution
- Monthly revenue vs target
- Monthly orders vs target
- Monthly returns vs target
- Most ordered product type
- Most returned product type

![Sales Overview](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132636.png?raw=true)

---

### 2. Regional Analysis

The regional analysis page provides a geographic view of order performance across different markets.

Features include:

- Geographic order distribution
- Country-level order analysis
- Region filters
- Europe
- North America
- Pacific
- Interactive map visualization

![Regional Analysis](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132810.png?raw=true)

---

### 3. Product Performance

The product analysis page allows individual products to be selected and evaluated against business targets.

Key metrics include:

- Product orders
- Product revenue
- Product profit
- Product return rate
- Monthly performance trends
- Return trends
- Order vs target
- Revenue vs target
- Profit vs target

The page also uses a dynamic metric selector to switch between:

- Orders
- Profit
- Returns
- Revenue
- Return Rate

![Product Analysis](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132824.png?raw=true)

---

### 4. Customer Analysis

The customer analysis page focuses on customer-level performance and revenue contribution.

Key metrics and analysis include:

- Total customers
- Average revenue per customer
- Revenue trends
- Customer income segmentation
- Customer occupation segmentation
- Customer-level order analysis
- Customer-level revenue analysis
- Top customer by revenue

![Customer Analysis](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132839.png?raw=true)

---

### 5. Custom Tooltip

Custom report-page tooltips were created to provide additional context when users interact with dashboard visuals.

The tooltip provides contextual metrics such as:

- Total Orders
- Total Profit
- Total Returns
- Total Revenue
- Return Rate
- Weekly order trend

The tooltip combines KPI information with a supporting trend visualization, allowing users to inspect additional business context without leaving the main dashboard.

![Custom Tooltip](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132859.png?raw=true)

---

## Key Power BI Features Used

- Interactive slicers
- Cross-filtering
- Custom report-page tooltips
- KPI cards
- Gauge charts
- Line charts
- Area charts
- Donut charts
- Bar charts
- Geographic/map visualization
- Dynamic metric selection
- Target vs actual analysis
- Conditional formatting
- Interactive date-range filtering
- Product segmentation
- Customer segmentation
- Data-driven visual analysis

---

## Business Questions Addressed

The dashboard was designed to answer questions such as:

1. How is overall revenue performing?
2. How does profit compare with revenue?
3. Which product categories generate the most orders?
4. Which products contribute most to revenue?
5. Which products have the highest return contribution?
6. How are orders distributed geographically?
7. Which products are performing above or below target?
8. How is product return rate changing over time?
9. Which customers generate the most revenue?
10. How does revenue vary across customer income and occupation groups?
11. How does average revenue per customer change over time?
12. Which product types are most frequently ordered and returned?

---

## Tools & Technologies

- **Power BI**
- **DAX**
- **Power Query**
- **Data Modeling**
- **Data Visualization**
- **AdventureWorks Dataset**

---

## Project Outcome

The dashboard transforms transactional sales and returns data into an interactive analytical solution for monitoring business performance.

It enables users to:

- Monitor revenue, profit, orders, and return rate
- Analyze product and category performance
- Evaluate performance against targets
- Identify high-performing customers
- Analyze customer segments
- Investigate geographic order distribution
- Track return trends
- Explore detailed metrics through interactive filtering and custom tooltips

---

## Screenshots

### Data Model

![Data Model](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20134854.png?raw=true)

### Sales Overview

![Sales Overview](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132636.png?raw=true)

### Regional Analysis

![Regional Analysis](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132810.png?raw=true)

### Product Analysis

![Product Analysis](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132824.png?raw=true)

### Customer Analysis

![Customer Analysis](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026-09-09%20132839.png?raw=true)

### Custom Tooltip

![Custom Tooltip](https://github.com/Gautham-va/Adventure_work_Dashboard/blob/main/Screenshot%202026%2009-09%20132859.png?raw=true)
