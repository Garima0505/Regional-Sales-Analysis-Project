# Regional-Sales-Analysis-Project


This repository contains a data analysis project focused on cleaning, wrangling, and analyzing a comprehensive regional sales dataset. The primary tool used is a Jupyter Notebook (Sales_Analysis_1_8_25.ipynb), which processes raw Excel data into a unified format suitable for reporting and visualization.



### 📄 Project Overview
The goal of this project is to consolidate sales data from multiple disparate sources (sheets) to create a single source of truth for analysis. The notebook demonstrates a complete data engineering pipeline:

* Data Loading: Ingests raw data from a multi-sheet Excel workbook.

* Data Integration: Merges Sales Orders with Customers, Regions, States, Products, and Budgets using relational keys.

* Data Cleaning: Handles missing values, removes redundant columns, and standardizes column naming conventions.

* Feature Engineering: Aligns budget data specifically to the fiscal year 2017.

* Export: Outputs the processed data to a CSV file for further usage.



### 🛠️ Technologies Used
* Python 3.x

* Pandas: For data manipulation and aggregation.

* NumPy: For numerical operations.

* Matplotlib & Seaborn: Imported for potential data visualization tasks.

* Google Colab: The notebook is optimized for the Colab environment (includes Drive mounting).



### 📂 Dataset Structure
The project relies on an input file named Regional Sales Dataset.xlsx containing the following sheets:

* Sales Orders: Transactional sales data (Dates, Order Quantity, Unit Price, etc.).

* Customers: Customer names and IDs.

* Regions: Geographic region details (City, County, Population, Median Income).

* State Regions: Mapping of States to broader Regions (e.g., West, Midwest).

* Products: Product names and IDs.

* 2017 Budgets: Budget targets for specific products for the year 2017.



### 📊 Key Data Transformations

* Merging Strategy: The script uses Left Joins to enrich the central Sales Orders table with dimensions from other sheets.

* Budget Handling: The code specifically isolates 2017 data to map budget figures, ensuring accurate comparisons for that fiscal year while leaving other years' budget columns as NaN.

* Output: The final cleaned dataframe is exported as file.csv.



### 📈 Future Improvements

* Add exploratory data analysis (EDA) visualizations to show sales trends over time.

* Implement profitability analysis comparing Unit Price vs Total Unit Cost.

* Compare actual 2017 revenue against the 2017 Budgets.



### 📝 License
This project is open-source and available for educational and analytical purposes.
