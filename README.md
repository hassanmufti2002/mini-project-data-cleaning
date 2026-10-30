# Mini Project - Data Cleaning of Messy Sales Dataset

### Project Overview
This project is about cleaning a messy sales dataset as part of Data Science learning. The raw dataset had 185 rows with missing values, outliers, duplicates, inconsistent date formats, and non-standard text.

### Dataset
- **Raw Dataset:** `Messy_data.csv` (185 rows x 13 columns)
- **Cleaned Dataset:** `cleaned_sales_dataset.csv` (180 rows x 13 columns)

### Cleaning Steps Performed

1. **Handled Missing Values:**
   - Filled CustomerName, Gender, Region with 'Unknown' / Mode
   - Filled UnitPrice & Quantity with median & mean

2. **Handled Duplicates:**
   - Removed 2 duplicate rows

3. **Handled Outliers in UnitPrice:**
   - Used IQR Method to detect and remove outliers (3 rows removed)
   - Q1=0.99, Q3=2.99, Upper Limit

4. **Standardized Date Formats:**
   - Converted OrderDate to datetime: `dd-mm-yyyy` to `YYYY-MM-DD`

5. **Standardized Text Data:**
   - CustomerName: Title Case & stripped spaces
   - ProductCategory, PaymentMethod, ProductName: Standardized capitalization

6. **Data Validation & Feature Creation:**
   - Recalculated `TotalAmount = Quantity * UnitPrice`

### Tools Used
- Python
- Pandas, NumPy
- Google Colab
- GitHub for Version Control

### Files in Repo
- `Data_Cleaning_Mini_Project.ipynb` - Complete Python code with step-by-step cleaning
- `cleaned_sales_dataset.csv` - Final cleaned dataset ready for analysis
- `README.md` - Project documentation

### Result
Cleaned dataset reduced from 185 to 180 rows (100% clean, no missing, no duplicates, no outliers).

### Author
**Hassan Mufti** - Data Science Student
GitHub: @hassanmufti2002
