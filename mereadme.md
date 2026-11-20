# Task 2: SQL for Data Extraction & Business Analysis

## Project Overview
Analyzed the Superstore retail dataset using SQLite and Python (`pandas` + `SQLAlchemy`) to extract business insights across product performance, customer tiers, regional profitability, and discounting impact.

## Repository Files
- `task2_sql_analysis.ipynb`: Jupyter Notebook executing 10 business queries with outputs and insights.
- `superstore_queries.sql`: Standalone SQL script containing all queries.
- `db_utils.py`: Reusable Python database connection and query execution module.

## Key Business Insights
- **Top Revenue Concentration:** *Canon imageCLASS 2200 Advanced Copier* is the highest revenue generator, with **Technology** leading all categories in sales and overall net profit.
- **Sub-Category Loss Leaks:** Filtering via `GROUP BY` and `HAVING` confirms that **Tables**, **Bookcases**, and **Supplies** operate at a net financial loss despite steady order volumes.
- **Heavy Discount Threshold:** Orders discounted above **50%** consistently generate steep net losses across categories, highlighting the need for stricter discount caps.
- **Customer Value Tiering:** CTE-based segmentation (`WITH` + `CASE WHEN`) shows that **VIP** and **Regular** spenders drive a disproportionate share of revenue, with the **Consumer** segment leading total order volume and profit.
- **Regional & Seasonal Growth:** Multi-table `JOIN` analyses show that **West** and **East** regions anchor company profitability, while monthly trends peak sharply in **November** and **December**.
