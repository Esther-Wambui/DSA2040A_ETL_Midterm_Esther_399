# ETL Midterm Project – Esther 

## Project Overview
This project demonstrates a full ETL (Extract, Transform, Load) pipeline using Python and pandas. The goal is to clean, enrich and load sales order data from CSV files into structured databases.

## ETL Steps

### 1. Extract (`etl_extract.ipynb`)
- Loaded raw_data.csv and incremental_data.csv
- Explored data with .head() and .info() ,help in understanding the datasets
- Identified missing values,duplicate rows and data types
- Saved raw data to the `data/` folder

### 2. Transform (`etl_transform.ipynb`)
Applied at least 4 transformations to both datasets:
- Filled missing values (quantity, unit_price, customer_name, region)
- Created total_price = quantity * unit_price
- Converted `order_date` to datetime
- Added new column: region_status
- Performed dropping of irrelevate rows
- Removed duplicates
- Saved outputs to `transformed/`

### 3. Load (`etl_load.ipynb`)
- Loaded transformed CSVs into SQLite databases using sqlite3
- Previewed loaded data using SQL queries
- Saved databases to `loaded/` folder

-Transform phase was completed before loading the data.

## Tools Used
- Python
- Pandas
- SQLite (sqlite3)
- Jupyter Notebook

##  How to Run the Project
1. Open the project folder in VS Code or Jupyter Lab
2. Run etl_extract.ipynb to load and inspect raw data
3. Run etl_transform.ipynb to clean and enrich the data
4. Run etl_load.ipynb to store the data in SQLite
5. Check the `loaded/` folder for `.db` files

## Screenshots



