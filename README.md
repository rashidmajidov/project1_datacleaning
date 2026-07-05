# 🛒 E-Commerce Data Cleaning Project

This repository contains the data cleaning process for an e-commerce dataset. The goal of this task was to handle missing values, check for duplicates, and ensure data consistency for future analysis.

## 📂 Project Structure
* `data_cleaning.ipynb` - Jupyter Notebook containing the full cleaning steps and Python code.
* `cleaned_data.csv` - The final, clean version of the dataset.

## 🧹 Data Cleaning Steps Done
1. **Handling Missing Values in `CouponCode`**
   * **Action:** Replaced `NaN` values with `"No Coupon"`.
   * **Rationale:** A logical check proved that `TotalPrice == Quantity * UnitPrice` for these rows, confirming no discount was applied.
2. **Handling Duplicates in `CustomerID`**
   * **Action:** Retained all duplicate rows.
   * **Rationale:** Duplicate IDs are legitimate in this context, as they represent repeat purchases by the same customer.
3. **Value Consistency & Quality Check**
   * Verified all categorical and textual values; no anomalies or unintended tokens were detected across the dataset.

## 🛠️ Technologies Used
* Python 3
* Pandas
* NumPy