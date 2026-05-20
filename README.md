Project Overview:
This project focuses on cleaning and preparing raw sales data using Python and Pandas.
The dataset contained missing values, formatting issues, and required validation checks before analysis.
The main objective of this project is to ensure high-quality, clean, and consistent data for further analytics tasks.
Tools & Technologies Used:
1.Python
2.Pandas
3.Google Colab
4.Excel
dataset Information
The dataset contains:
Order details
Customer information
Product details
Payment methods
Coupon codes
Order status
Total price
Total Records: 1200
Total Columns: 14
Tasks Performed:
1. Data Loading
Imported dataset using Pandas.
2. Missing Value Handling
Identified missing values using:
1.df.isnull().sum()
Filled missing values in CouponCode column:
2.df['CouponCode'] = df['CouponCode'].fillna('No Coupon')
3. Duplicate Data Check
Checked duplicate rows:
df.duplicated().sum()
Removed duplicates:
df.drop_duplicates()
4. Duplicate ID Validation
Verified unique OrderID values:
df['OrderID'].duplicated().sum()
5. Date Formatting
Converted Date column into proper datetime format:
df['Date'] = pd.to_datetime(df['Date'])
6. Export Cleaned Dataset
Saved cleaned dataset:
Python
df.to_excel("cleaned_dataset.xlsx", index=False)
Project Results:
Missing values handled successfully
No duplicate rows found
Zero duplicate Order IDs
Date formats validated successfully
Cleaned dataset exported successfully
Project Files:
DataCleaningProject.ipynb
cleaned_dataset.xlsx
Conclusion:
This project demonstrates the complete workflow of data cleaning and preparation using Python Pandas.
The cleaned dataset is now ready for further data analysis and visualization tasks.
