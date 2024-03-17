# E-commerce-Data-Pipeline

**Introduction**
This project aims to analyze supply and demand trends around holidays using e-commerce data. We built a data pipeline to extract, transform, aggregate, and load data from two main sources: a PostgreSQL database containing grocery_sales table and a extra_data.parquet file with complementary information.

**Project Overview**
Extract Data: We combined data from grocery_sales table and extra_data.parquet file to create a merged DataFrame named merged_df.

Transform Data: The transform() function filled missing values, added a "Month" column, filtered sales over $10,000, and dropped unnecessary columns to create clean_data.

Aggregate Data: The avg_monthly_sales() function aggregated clean_data to calculate average monthly sales, stored in agg_data.

Load Data: Data was saved as CSV files (clean_data.csv and agg_data.csv) without an index using the load() function.

Validation: The validation() function checked the existence of CSV files in the current directory.

**Conclusion**
This data pipeline streamlines e-commerce data handling, aiding supply chain management and sales forecasting. Automation ensures data consistency and reliability for further analysis and insights generation.
