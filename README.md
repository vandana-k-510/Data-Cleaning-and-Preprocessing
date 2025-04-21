Amazon Sales Dataset - Data Cleaning Project
Objective
The goal of this project was to clean and prepare the Amazon Sales raw dataset for analysis by handling missing values, duplicates, inconsistent formats, and ensuring data types are correct.

Tools Used
Python (Pandas)

Jupyter Notebook / Google Colab (optional)

Excel (for quick verification)

Steps Performed
1. Handling Missing Values
Checked for missing values using .isnull().sum().

Handled missing data appropriately:

Dropped rows where critical information was missing.

For non-critical fields, filled missing values if necessary.

2. Removing Duplicates
Identified duplicate rows using .duplicated().

Removed duplicate rows with .drop_duplicates() to ensure each entry is unique.

3. Standardizing Text Formats
Standardized text data:

Trimmed extra spaces.

Converted all string columns (like Country, Category, etc.) to lowercase.

Corrected inconsistencies in fields like country names or product categories.

4. Date Formatting
Converted the order date column into a consistent dd-mm-yyyy format using pd.to_datetime().

5. Renaming Columns
Renamed column headers to be clean and consistent:

Changed all column names to lowercase.

Replaced spaces with underscores (_) for easier programming.

6. Fixing Data Types
Ensured numeric columns (like sales, quantity, profit, etc.) are in the correct int or float format.

Converted date columns to proper datetime objects.

Verified that categorical columns remain as object dtype.
