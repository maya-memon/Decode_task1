# Project 1: Data Cleaning & Preparation

## Project Overview
This project focuses on cleaning, verifying, and preparing a transactional dataset containing 1,200 records. Data cleaning is a crucial first step in any data analysis workflow to ensure accuracy, consistency, and reliability of insights.

## Dataset Summary
- **Total Records:** 1,200
- **Initial Missing Values:** 309 (Found exclusively in the `CouponCode` column)
- **Duplicate Rows:** 0
- **Duplicate OrderID:** 0
- **Date Format:** Verified and found valid.
- **Mathematical Consistency:** Validated (`TotalPrice` = `Quantity` × `UnitPrice` for all rows).

## Cleaning Steps Performed
1. **Handling Missing Data:** Replaced 309 missing (NaN) values in the `CouponCode` column with the string `"No Coupon"`.
2. **Deduplication:** Scanned the dataset for overall duplicate rows and unique `OrderID` violations; no duplicates were found.
3. **Data Type & Format Verification:** Validated that date columns conform to standard datetime formats.
4. **Calculated Field Validation:** Programmatically cross-checked that `TotalPrice` matches the product of `Quantity` and `UnitPrice` across all 1,200 records.

## Files Delivered
- `Cleaned_Dataset_Project1.xlsx` - The final, clean, and processed dataset ready for analysis.

## Tools Used
- **Language:** Python 3.x
- **Libraries:** Pandas, OpenPyXL (for Excel export)
