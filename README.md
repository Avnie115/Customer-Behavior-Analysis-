# Customer-Behavior-Analysis-

An end-to-end data analytics project transforming raw retail data into actionable business intelligence. Utilizing **Python** for automated ETL and cleaning, **PostgreSQL** for complex behavioral querying, **Power BI** for visual analytics, and professional **Business Reports/PPTs** for stakeholder communication.

## 📌 Project Overview
This project analyzes transactional data from **3,900 purchases** to uncover deep insights into customer spending patterns, segmentation, and subscription health. By integrating data engineering and business analytics, the project provides a strategic roadmap for increasing customer retention and optimizing revenue.

## 🛠️ Tech Stack & Tools
* **Data Engineering:** Python (Pandas) for ETL, data cleaning, and feature engineering.
* **Database Management:** PostgreSQL for structured data storage and complex business querying.
* **Data Visualization:** Power BI for building interactive executive dashboards.
* **Documentation:** Professional Business Reporting for stakeholder communication.

## 🚀 Key Features & Workflow

### 1. Data Cleaning & Engineering (Python)
* **Imputation:** Handled 37 missing values in the `Review Rating` column using category-specific median imputation to maintain statistical integrity.
* **Standardization:** Transformed column headers to `snake_case` for database standardization and readability.
* **Feature Engineering:** Created `age_group` bins and converted qualitative purchase frequencies into numeric day-intervals for precise analysis.
* **Optimization:** Streamlined the dataset by removing redundant features like `promo_code_used`.

### 2. Business Logic & Querying (SQL)
Designed and executed 10+ complex SQL queries to solve specific business problems, including:
* **Revenue Analysis:** Comparing performance across Gender and Age Groups.
* **Customer Segmentation:** Classifying users into **New**, **Returning**, and **Loyal** tiers based on historical purchase frequency.
* **Behavioral Audits:** Analyzing the conversion funnel from repeat buyers to active subscribers.
* **Product Insights:** Identifying "Discount-Dependent" products and top-rated items by category.

### 3. Visual Analytics (Power BI)
Developed a high-fidelity dashboard to track:
* **KPIs:** Total Customers (3.9K), Average Purchase Amount ($59.76), and Average Review Rating (3.75).
* **Demographics:** Revenue distribution by Age Group and Gender.
* **Market Share:** Subscription status breakdown (27% Yes vs. 73% No).

## 📊 Key Findings
* **The "Loyal" Core:** The business maintains a strong base of **3,116 Loyal customers**, indicating high satisfaction and retention.
* **Subscription Gap:** Despite similar spending habits, there is a massive opportunity to convert over **2,500 repeat buyers** into the subscription program.
* **Price Sensitivity:** Products like **Hats and Sneakers** are highly discount-dependent, with nearly 50% of sales occurring during promotions.

## 💡 Business Recommendations
* **Targeted Conversion:** Launch a loyalty-to-subscription campaign for the high-volume "Returning" segment.
* **Inventory Optimization:** Use "Discount-Dependent" products as loss-leaders to drive traffic for high-margin items.
* **Premium Upselling:** Leverage Express Shipping trends to offer tiered shipping incentives.

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
