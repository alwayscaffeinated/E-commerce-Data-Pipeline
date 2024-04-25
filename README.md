# E-commerce-Data-Pipeline

_**Introduction**_

This project aims to analyze supply and demand trends around holidays using e-commerce data.Built a data pipeline to extract, transform, aggregate, and load data from two main sources: a PostgreSQL database containing grocery_sales table and a extra_data.parquet file with complementary information.

_**Project Overview**_

_Extract Data:_ We combined data from grocery_sales table and extra_data.parquet file to create a merged DataFrame named merged_df.

_Transform Data:_ The transform() function filled missing values, added a "Month" column, filtered sales over $10,000, and dropped unnecessary columns to create clean_data.

_Aggregate Data:_ The avg_monthly_sales() function aggregated clean_data to calculate average monthly sales, stored in agg_data.

_Load Data:_ Data was saved as CSV files (clean_data.csv and agg_data.csv) without an index using the load() function.

_Validation:_ The validation() function checked the existence of CSV files in the current directory.

_**Conclusion**_

This data pipeline streamlines e-commerce data handling, aiding supply chain management and sales forecasting. Automation ensures data consistency and reliability for further analysis and insights generation.
