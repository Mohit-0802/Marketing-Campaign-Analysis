Task 1 - Data Cleaning and Preprocessing

Objective

Clean and prepare a raw marketing campaign dataset that had missing values,
duplicates, inconsistent formats, and outliers.

Dataset

	•	Name: Customer Personality Analysis (Marketing Campaign)
	•	Records: 2,240 (raw) → 2,232 (cleaned)
	•	Columns: 35 (raw) → 29 (cleaned)

Tool Used

Microsoft Excel

Steps Performed

	1.	Removed empty columns — Deleted 6 unnamed, completely empty columns
(35 columns reduced to 29).
	2.	Standardized date format — Fixed the dt_customer column, which had mixed
formats (datetime objects + text strings). Converted all values to dd-mm-yyyy format.
	3.	Cleaned marital_status column — Removed 4 rows with invalid values
(Absurd, YOLO). Replaced "Alone" with "Single" for consistency.
	4.	Removed outlier birth years — Deleted 3 rows with birth years
1893, 1899 and 1900, which are clearly impossible/erroneous.
	5.	Removed income outlier — Deleted 1 row with income = 6,66,666,
which was a data entry error (all others below 1,62,000).
	6.	Cleared blank rows — Removed 4 completely empty spreadsheet rows left in the
sheet after the deletions. These were empty rows, not customer records, so they
do not change the record count.

Record Reconciliation

Step	Records removed	Records remaining
Raw dataset	–	2,240
Invalid marital status (Absurd, YOLO)	4	2,236
Impossible birth years (1893, 1899, 1900)	3	2,233
Income outlier (666,666)	1	2,232
Cleaned dataset	8 in total	2,232

Result

	•	Raw dataset: 2,240 records, 35 columns
	•	Cleaned dataset: 2,232 records, 29 columns
	•	No missing values, no duplicate rows; marital_status contains only
Married, Together, Single, Divorced and Widow
	•	File: marketing_campaign_CLEANED.xlsx
