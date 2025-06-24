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

## Screenshots showing the codes and outputs of the whole process are below: 
### extracting
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_45_51](https://github.com/user-attachments/assets/c2800bf8-faf3-44dd-9897-588037557d7c)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_51_28](https://github.com/user-attachments/assets/4ac48c59-9e97-4de0-a0b6-18ad3308241d)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_51_41](https://github.com/user-attachments/assets/b36c6548-f54d-41c4-add0-0bc97ec02dd0)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_51_48](https://github.com/user-attachments/assets/afe5f037-23dc-4866-a4f1-acd891b7879b)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_51_57](https://github.com/user-attachments/assets/26325048-d3e8-41d5-b109-ae0f75f14a60)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_52_30](https://github.com/user-attachments/assets/714fb6e5-4a86-4bdc-9e91-04177d16bdbb)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_52_53](https://github.com/user-attachments/assets/ce07196c-dfdb-456a-8c12-bdbb5c1b3818)
### Transforming
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_53_20](https://github.com/user-attachments/assets/b6aabe90-f154-483a-834d-ee9d422c7a20)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_53_37](https://github.com/user-attachments/assets/4b6b6c62-32a5-4a03-a6cc-392978d14bb4)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_53_47](https://github.com/user-attachments/assets/3d95a99e-ca33-4253-8494-ef8cb99060d9)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_54_19](https://github.com/user-attachments/assets/66c37a36-d740-4299-b578-60f648af9abd)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_54_19](https://github.com/user-attachments/assets/21f62a1e-b0ee-4018-b5ba-79f8fbba064d)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_54_33](https://github.com/user-attachments/assets/6db6c12c-6835-43f5-b075-4e2b2e05a841)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_54_46](https://github.com/user-attachments/assets/3beab594-db09-4702-95b5-66dade2ba2da)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_54_55](https://github.com/user-attachments/assets/f65667ed-d2b7-44a0-afcb-ae8406615151)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_55_13](https://github.com/user-attachments/assets/76ee7621-6a08-4fc8-a80d-0d0f63fa8655)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_55_37](https://github.com/user-attachments/assets/62f2c5ff-384e-4633-b115-62d65671145c)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_55_57](https://github.com/user-attachments/assets/5b0bb4e4-5962-4fd4-9339-be6465afe421)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_56_09](https://github.com/user-attachments/assets/45484c1e-8735-423e-ab1a-6ef34f7c04ef)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_56_20](https://github.com/user-attachments/assets/edee0cd0-9079-43d1-b01a-0de78781b40e)
![etl_extract ipynb - ETL_Midterm_Esther_399 - Visual Studio Code 24_06_2025 18_56_25](https://github.com/user-attachments/assets/cbed8d68-9bcd-42c5-a2e3-261c4e47e8c7)







