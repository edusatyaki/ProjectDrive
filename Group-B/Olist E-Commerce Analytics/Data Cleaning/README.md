# Olist Brazilian E-Commerce Dataset
## Data Cleaning and Preprocessing

---

## 1. Project Description

The objective of this project is to clean and preprocess the Olist Brazilian E-Commerce Dataset before performing Exploratory Data Analysis (EDA), visualization, and predictive modeling. Data preprocessing is one of the most important phases of the data analytics lifecycle because the quality of the input data directly affects the accuracy of the analysis and machine learning models.

The raw datasets contain issues such as duplicate records, missing values, inconsistent formatting, and incorrect data types. These issues were identified through exploratory analysis and systematically resolved using appropriate data cleaning techniques while preserving meaningful business information.

---

## 2. Dataset Information

The project consists of nine datasets, each representing a different aspect of the e-commerce platform.

| Dataset | Description |
|----------|-------------|
| olist_customers_dataset.csv | Customer information |
| olist_geolocation_dataset.csv | Customer and seller geographical information |
| olist_order_items_dataset.csv | Products purchased in each order |
| olist_order_payments_dataset.csv | Payment details |
| olist_order_reviews_dataset.csv | Customer reviews and ratings |
| olist_orders_dataset.csv | Order information |
| olist_products_dataset.csv | Product details |
| olist_sellers_dataset.csv | Seller information |
| product_category_name_translation.csv | Portuguese to English category translation |

---

## 3. Software Requirements

The following software and libraries were used throughout the project:

- Python 3.12
- Google Colab
- Pandas
- NumPy
- OS Module

---

## 4. Data Cleaning Methodology

The preprocessing workflow followed a structured sequence to ensure the datasets became accurate, consistent, and suitable for analysis.

### Step 1 – Import Required Libraries

The required Python libraries were imported to support data loading, manipulation, preprocessing, and validation.

---

### Step 2 – Load the Dataset

All CSV files were loaded into individual Pandas DataFrames from Google Drive.

---

### Step 3 – Dataset Exploration

The datasets were explored to understand their overall structure by examining:

- Dataset dimensions
- Column names
- Data types
- Summary statistics
- Missing values
- Duplicate records

---

### Step 4 – Remove Duplicate Records

Duplicate records were identified within the Geolocation dataset and removed to eliminate redundant information while preserving unique geographical records.

---

### Step 5 – Handle Missing Values

Missing values were handled according to the nature of each dataset.

**Order Reviews Dataset**

- Missing review titles were replaced with **"No Title"**.
- Missing review messages were replaced with **"No Review"**.

**Products Dataset**

- Missing product categories were replaced with **"Unknown"**.
- Missing numerical attributes were filled using the median value of their respective columns.

---

### Step 6 – Convert Data Types

All date-related columns were converted from object data type to datetime format.

The following datasets were updated:

- Orders
- Order Reviews
- Order Items

This conversion enables chronological analysis and date calculations.

---

### Step 7 – Trim White Spaces

Leading and trailing white spaces were removed from selected text columns to improve data consistency.

The affected datasets include:

- Customers
- Sellers
- Products
- Geolocation

---

### Step 8 – Validate the Cleaned Data

After completing all preprocessing operations, the datasets were validated by checking:

- Missing values
- Duplicate records
- Data types
- Dataset dimensions

This validation ensured that the cleaning process was successfully completed.

---

### Step 9 – Generate the Cleaning Log

A detailed Data Cleaning Log was created to document every preprocessing activity, including:

- Cleaning operation
- Dataset affected
- Description
- Cleaning status

The cleaning log provides transparency and improves project reproducibility.

---

### Step 10 – Export Cleaned Datasets

The cleaned datasets were exported as new CSV files for future analysis and visualization.

The original datasets remained unchanged.

---

## 5. Validation Summary

After preprocessing, the following results were obtained:

- Duplicate records were removed successfully.
- Missing values were handled appropriately.
- Date columns were converted successfully.
- White spaces were removed from text columns.
- Data types were verified.
- Dataset integrity was maintained.

The remaining missing values within the Orders dataset were intentionally retained because they correspond to cancelled, unavailable, or undelivered orders. These values represent valid business information rather than data quality issues.

---

## 6. Output Files

The project generates the following output files:

- Cleaned CSV datasets
- Data Cleaning Log (PDF)
- README.md

## 8. Conclusion

The data cleaning and preprocessing process significantly improved the overall quality of the Olist Brazilian E-Commerce Dataset. Duplicate records were removed, missing values were handled appropriately, date columns were converted to the correct format, and text fields were standardized. The cleaned datasets were successfully validated and are now ready for exploratory data analysis, dashboard development, statistical analysis, feature engineering, and machine learning applications while preserving important business information.
