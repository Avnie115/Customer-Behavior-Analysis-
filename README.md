# Customer-Behavior-Analysis-

An end-to-end data analytics project transforming raw retail data into actionable business intelligence. [cite_start]Utilizing **Python** for automated ETL and cleaning, **PostgreSQL** for complex behavioral querying, **Power BI** for visual analytics, and professional **Business Reports/PPTs** for stakeholder communication. [cite: 3, 4, 13, 25, 27, 63]

## 📌 Project Overview
[cite_start]This project analyzes transactional data from **3,900 purchases** to uncover deep insights into customer spending patterns, segmentation, and subscription health. [cite: 3] [cite_start]By integrating data engineering and business analytics, the project provides a strategic roadmap for increasing customer retention and optimizing revenue. [cite: 4]

## 🛠️ Tech Stack & Tools
* [cite_start]**Data Engineering:** Python (Pandas) for ETL, data cleaning, and feature engineering. [cite: 13, 15]
* [cite_start]**Database Management:** PostgreSQL for structured data storage and complex business querying. [cite: 25, 27]
* [cite_start]**Data Visualization:** Power BI for building interactive executive dashboards. [cite: 63]
* [cite_start]**Documentation:** Professional Business Reporting for stakeholder communication. [cite: 1, 98]

## 🚀 Key Features & Workflow

### 1. Data Cleaning & Engineering (Python)
* [cite_start]**Imputation:** Handled 37 missing values in the `Review Rating` column using category-specific median imputation to maintain statistical integrity. [cite: 12, 19]
* [cite_start]**Standardization:** Transformed column headers to `snake_case` for database standardization and readability. [cite: 20]
* [cite_start]**Feature Engineering:** Created `age_group` bins and converted qualitative purchase frequencies into numeric day-intervals for precise analysis. [cite: 21, 22, 23]
* [cite_start]**Optimization:** Streamlined the dataset by removing redundant features like `promo_code_used`. [cite: 24]

### 2. Business Logic & Querying (SQL)
Designed and executed 10+ complex SQL queries to solve specific business problems, including:
* [cite_start]**Revenue Analysis:** Comparing performance across Gender and Age Groups. [cite: 28, 60]
* [cite_start]**Customer Segmentation:** Classifying users into **New**, **Returning**, and **Loyal** tiers based on historical purchase frequency. [cite: 53]
* [cite_start]**Behavioral Audits:** Analyzing the conversion funnel from repeat buyers to active subscribers. [cite: 58]
* [cite_start]**Product Insights:** Identifying "Discount-Dependent" products and top-rated items by category. [cite: 42, 50]

### 3. Visual Analytics (Power BI)
[cite_start]Developed a high-fidelity dashboard to track: [cite: 62, 63]
* [cite_start]**KPIs:** Total Customers (3.9K), Average Purchase Amount ($59.76), and Average Review Rating (3.75). [cite: 68, 70, 72]
* [cite_start]**Demographics:** Revenue distribution by Age Group and Gender. [cite: 88, 74]
* [cite_start]**Market Share:** Subscription status breakdown (27% Yes vs. 73% No). [cite: 80, 90]

## 📊 Key Findings
* [cite_start]**The "Loyal" Core:** The business maintains a strong base of **3,116 Loyal customers**, indicating high satisfaction and retention. [cite: 54]
* [cite_start]**Subscription Gap:** Despite similar spending habits, there is a massive opportunity to convert over **2,500 repeat buyers** into the subscription program. [cite: 49, 59]
* [cite_start]**Price Sensitivity:** Products like **Hats and Sneakers** are highly discount-dependent, with nearly 50% of sales occurring during promotions. [cite: 52]

## 💡 Business Recommendations
* [cite_start]**Targeted Conversion:** Launch a loyalty-to-subscription campaign for the high-volume "Returning" segment. [cite: 99, 102]
* [cite_start]**Inventory Optimization:** Use "Discount-Dependent" products as loss-leaders to drive traffic for high-margin items. [cite: 103, 104]
* [cite_start]**Premium Upselling:** Leverage Express Shipping trends to offer tiered shipping incentives. [cite: 46, 105]

## ⚙️ How to Run

### 1. Prerequisites
Ensure you have the following installed:
* Python 3.x
* PostgreSQL
* Power BI Desktop
* Python Libraries: `pandas`, `sqlalchemy`, `psycopg2-binary`

### 2. Data Cleaning (Python)
1.  Navigate to the `scripts/` folder.
2.  Open `data_analysis_jupyter.ipynb` in Jupyter Notebook or VS Code.
3.  Update the database credentials in the `create_engine` section to match your local PostgreSQL setup (Username, Password, Port).
4.  Run all cells to perform cleaning, feature engineering, and automated loading into your SQL database.

### 3. Database Analysis (SQL)
1.  Open your SQL editor (e.g., pgAdmin).
2.  Execute the queries found in `customer_behavior_postgreSQL_queries.sql`.
3.  These queries generate core business insights, such as customer segments and revenue contribution.

### 4. Visualization (Power BI)
1.  Open the `.pbix` file located in the `dashboard/` folder.
2.  If prompted, refresh the data source to link it to your local PostgreSQL table.
3.  Explore the visual KPIs and interactive charts.
