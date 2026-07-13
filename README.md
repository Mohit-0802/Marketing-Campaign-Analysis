# Task 1 - Data Cleaning and Preprocessing

## Objective
Clean and prepare a raw marketing campaign dataset that had missing values, 
duplicates, inconsistent formats, and outliers.

## Dataset
- Name: Customer Personality Analysis (Marketing Campaign)
- Rows: 2240 | Columns: 35 (raw) → 29 (cleaned)

## Tool Used
Microsoft Excel

## Steps Performed

1. **Removed empty columns** — Deleted 6 unnamed empty columns (AD to AJ)

2. **Standardized date format** — Fixed dt_customer column which had mixed 
   formats (datetime objects + text strings). Converted all to dd-mm-yyyy format.

3. **Cleaned marital_status column** — Removed rows with invalid values 
   (Absurd, YOLO). Replaced "Alone" with "Single" for consistency.

4. **Removed outlier birth years** — Deleted 3 rows with birth years 
   1893, 1899, 1900 which are clearly impossible/erroneous.

5. **Removed income outlier** — Deleted 1 row with income = 6,66,666 
   which was a data entry error (all others below 1,62,000).

6. **Removed blank rows** — Deleted 4 completely empty rows left after cleaning.

## Result
- Raw dataset: 2240 rows, 35 columns
- Cleaned dataset: 2236 rows, 29 columns
- File: marketing_campaign_CLEANED.xlsx
