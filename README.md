# Large-Scale Data Processing with Apache Spark

PySpark pipeline processing 1M+ row e-commerce dataset with aggregations, 
window functions, and KPI computation. Output saved to Parquet and CSV.

## Tech Stack
- Apache Spark 4.0.2 (PySpark)
- Python
- Google Colab
- Parquet (output format)

## What It Does
1. Generates 1,000,000 rows of synthetic e-commerce sales data
2. Loads into Spark DataFrame and caches for performance
3. Cleans data — null handling, deduplication, validation
4. Computes KPIs:
   - Revenue and profit by product category
   - Customer Lifetime Value (top 10,000 customers)
   - Monthly revenue trends (2021–2024)
   - Cumulative revenue using window functions
   - Top 3 customers per region using RANK() window function
5. Saves output to Parquet (1M rows) and CSV (aggregated KPIs)

## Key Results
- Total Revenue (2021–2024): ~$3.7 Billion
- Best performing category: Clothing ($746M)
- Top customer LTV: $587,693
- All 5 regions analyzed with ranked customer segments

## Files
- `spark_data_processing.ipynb` — Full PySpark notebook with all transformations and KPIs