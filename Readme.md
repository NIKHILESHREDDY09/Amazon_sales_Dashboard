## Amazon Retail Sales Dashboard – Business Performance Analysis

### Project Overview

This project focuses on analyzing retail sales data and transforming it into actionable business insights using Power BI. The goal of the dashboard is to provide a clear view of overall business performance, product demand, store-level contribution, and revenue trends over time.

Instead of looking at raw sales data, this dashboard helps decision-makers quickly understand **what is selling, where revenue is coming from, and how sales performance changes across time and store formats.**

The report is designed to be interactive so users can filter results by **sales roles and customer segments**, allowing deeper analysis of different parts of the business.

---

### Key Business Metrics

At the top of the dashboard, four key metrics provide an instant overview of the business:

* **Total Revenue:** ₹2.75 Billion generated from all transactions
* **Total Stores:** 500 retail locations contributing to sales
* **Total Sales:** 1 Million transactions processed
* **Total Customers:** 100,000 unique customers served

These KPIs help stakeholders quickly understand the scale of the business and overall performance.

---

### Product Performance Insights

The **Top 10 Products** chart highlights which products contribute the most to overall sales.

From the analysis, products such as **Running Shoes, Yoga Mats, and Tennis Rackets** are among the top performers. This suggests strong demand in the sports and fitness category. Other items like **Smart Fridges and Book Shelves** also contribute consistently, indicating steady demand in home-related product segments.

Insights like this can help business teams make better decisions around **inventory planning, product promotions, and demand forecasting**.

---

### Store Category Sales Comparison

The **Total Sales by Store Category** chart compares transaction volumes across different retail formats.

The data shows that **Supermarkets generate the highest number of transactions**, followed closely by **Small Stores and Shops**. **Large Malls and Complexes** contribute slightly fewer transactions.

This type of comparison helps businesses understand how different store formats perform and where customer activity is concentrated.

---

### Weekly Revenue Trends

The **Total Revenue by Week** chart provides a time-based view of sales performance across the year.

Several revenue spikes appear during specific weeks, which could be associated with seasonal demand, promotional campaigns, or major shopping periods. At the same time, some weeks show stable revenue levels, representing consistent baseline demand.

Tracking revenue trends like this helps businesses identify **high-performing periods, forecast demand, and plan marketing campaigns more effectively.**

---

### Revenue Distribution by Store Type

The **Revenue by Store Type** visualization shows how different store formats contribute to overall revenue.

The contribution is relatively balanced:

* **Supermarkets:** ~34.6% of total revenue
* **Small Stores / Shops:** ~33.7%
* **Large Malls / Complexes:** ~31.7%

This balanced distribution indicates that revenue is not dependent on a single store type, which is a healthy sign for retail stability.

---

### Interactive Analysis

The dashboard includes filters that allow users to explore the data in more detail:

**Sales Role Filter**
Allows analysis of performance based on the role of sales personnel.

**Customer Segment Filter**
Allows stakeholders to analyze how different customer groups contribute to sales.

These filters help users quickly move from a high-level overview to more detailed insights.

---

### Tools and Technologies

* **Power BI** for dashboard development and visualization
* **Star Schema Data Model** for efficient analytics
* **DAX Measures** for calculating business metrics
* **Interactive Filters and Slicers** for flexible exploration

---

### Final Thoughts

This dashboard demonstrates how raw transactional data can be transformed into meaningful insights that support better business decisions. By combining product analysis, store comparisons, and revenue trends, the report provides a clear picture of retail performance and highlights areas where businesses can optimize operations and strategy.

## Data Modeling (Star Schema)

Before building the dashboard, the dataset was structured using a **Star Schema data model** to optimize analytical performance and simplify reporting.

The model consists of one central **fact table** containing transactional sales data, surrounded by several **dimension tables** that provide descriptive business attributes.

### Fact Table

**fact_sales_normalized**

This is the core transactional table that stores measurable business events.

Key fields include:

* sales amount
* product identifier
* customer identifier
* store identifier
* campaign identifier
* sales date

Each record represents a **single sales transaction**, which allows flexible aggregation across multiple business dimensions.

---

### Dimension Tables

**dim_products**
Contains product-level information such as:

* product name
* product category
* brand
* origin location

This table enables analysis of **product performance and category-level trends**.

---

**dim_customers**
Stores customer-related attributes including:

* customer segment
* customer identifiers

This dimension allows segmentation of revenue and sales behavior across different customer groups.

---

**dim_stores**
Provides store-level details such as:

* store name
* store location
* store type (Supermarkets, Small Stores, Large Malls)

This dimension is used to analyze how different retail formats contribute to revenue.

---

**dim_salespersons**
Contains information about sales personnel including:

* salesperson name
* salesperson role

This allows performance analysis by different sales roles.

---

**dim_campaigns**
Stores marketing campaign information such as:

* campaign name
* campaign budget
* campaign start and end dates

This enables potential analysis of marketing effectiveness.

---

**dim_dates (Calendar Table)**
Provides time-related attributes including:

* full date
* week number
* month
* quarter

This table supports **time-based analysis such as weekly revenue trends and seasonal patterns**.

---

### Why Star Schema?

The star schema structure was chosen because it:

* Improves **query performance in analytical workloads**
* Simplifies **relationships between business entities**
* Makes **Power BI calculations and aggregations more efficient**
* Provides a clean separation between **measurable facts and descriptive attributes**

This modeling approach ensures that the dashboard can scale efficiently as additional data or analytical requirements are introduced.
## Amazon Retail Sales Dashboard – Business Performance Analysis

### Project Overview

This project focuses on analyzing retail sales data and transforming it into actionable business insights using Power BI. The goal of the dashboard is to provide a clear view of overall business performance, product demand, store-level contribution, and revenue trends over time.

Instead of looking at raw sales data, this dashboard helps decision-makers quickly understand **what is selling, where revenue is coming from, and how sales performance changes across time and store formats.**

The report is designed to be interactive so users can filter results by **sales roles and customer segments**, allowing deeper analysis of different parts of the business.

---

### Key Business Metrics

At the top of the dashboard, four key metrics provide an instant overview of the business:

* **Total Revenue:** ₹2.75 Billion generated from all transactions
* **Total Stores:** 500 retail locations contributing to sales
* **Total Sales:** 1 Million transactions processed
* **Total Customers:** 100,000 unique customers served

These KPIs help stakeholders quickly understand the scale of the business and overall performance.

---

### Product Performance Insights

The **Top 10 Products** chart highlights which products contribute the most to overall sales.

From the analysis, products such as **Running Shoes, Yoga Mats, and Tennis Rackets** are among the top performers. This suggests strong demand in the sports and fitness category. Other items like **Smart Fridges and Book Shelves** also contribute consistently, indicating steady demand in home-related product segments.

Insights like this can help business teams make better decisions around **inventory planning, product promotions, and demand forecasting**.

---

### Store Category Sales Comparison

The **Total Sales by Store Category** chart compares transaction volumes across different retail formats.

The data shows that **Supermarkets generate the highest number of transactions**, followed closely by **Small Stores and Shops**. **Large Malls and Complexes** contribute slightly fewer transactions.

This type of comparison helps businesses understand how different store formats perform and where customer activity is concentrated.

---

### Weekly Revenue Trends

The **Total Revenue by Week** chart provides a time-based view of sales performance across the year.

Several revenue spikes appear during specific weeks, which could be associated with seasonal demand, promotional campaigns, or major shopping periods. At the same time, some weeks show stable revenue levels, representing consistent baseline demand.

Tracking revenue trends like this helps businesses identify **high-performing periods, forecast demand, and plan marketing campaigns more effectively.**

---

### Revenue Distribution by Store Type

The **Revenue by Store Type** visualization shows how different store formats contribute to overall revenue.

The contribution is relatively balanced:

* **Supermarkets:** ~34.6% of total revenue
* **Small Stores / Shops:** ~33.7%
* **Large Malls / Complexes:** ~31.7%

This balanced distribution indicates that revenue is not dependent on a single store type, which is a healthy sign for retail stability.

---

### Interactive Analysis

The dashboard includes filters that allow users to explore the data in more detail:

**Sales Role Filter**
Allows analysis of performance based on the role of sales personnel.

**Customer Segment Filter**
Allows stakeholders to analyze how different customer groups contribute to sales.

These filters help users quickly move from a high-level overview to more detailed insights.

---

### Tools and Technologies

* **Power BI** for dashboard development and visualization
* **Star Schema Data Model** for efficient analytics
* **DAX Measures** for calculating business metrics
* **Interactive Filters and Slicers** for flexible exploration

---

### Final Thoughts

This dashboard demonstrates how raw transactional data can be transformed into meaningful insights that support better business decisions. By combining product analysis, store comparisons, and revenue trends, the report provides a clear picture of retail performance and highlights areas where businesses can optimize operations and strategy.
