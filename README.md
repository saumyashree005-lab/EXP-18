# NAME : SAUMYA SHREE PRN: 25070123161

# THEORY:

Data preprocessing is an important step in data analysis and machine learning. It involves cleaning, transforming, and organizing raw data into a usable format. This includes handling missing values, scaling data, encoding categorical variables, and improving data quality.
Python libraries like pandas, numpy, and sklearn are widely used for preprocessing tasks.

# FUNCTIONS AND COMMANDS USED:
1. Importing Libraries
import pandas as pd → Used for data manipulation and analysis.
import numpy as np → Used for numerical operations.
from sklearn.preprocessing import MinMaxScaler, StandardScaler → Used for data scaling.
2. Loading Dataset
pd.read_csv("file.csv") → Loads dataset into a DataFrame.
3. Basic Data Exploration
df.head() → Displays first 5 rows.
df.tail() → Displays last 5 rows.
df.shape → Returns number of rows and columns.
df.info() → Gives summary of dataset.
df.describe() → Shows statistical summary.
4. Handling Missing Values
df.isnull().sum() → Counts missing values in each column.
df.dropna() → Removes rows with missing values.
df.fillna(value) → Fills missing values with a specified value.
5. Data Transformation
Min-Max Scaling:
MinMaxScaler() → Scales values between 0 and 1.
scaler.fit_transform(df[['column']])
Standardization:
StandardScaler() → Transforms data to mean = 0 and standard deviation = 1.
scaler.fit_transform(df[['column']])
6. Encoding Categorical Data
pd.get_dummies(df['column']) → Converts categorical data into numerical format (one-hot encoding).
7. Removing Duplicates
df.duplicated().sum() → Counts duplicate rows.
df.drop_duplicates() → Removes duplicate rows.
8. Filtering Data
df.loc[] → Select rows based on conditions.
df[df['column'] == value] → Filters specific rows.
9. Sorting Data
df.sort_values(by='column') → Sorts data based on column values.
10. Feature Selection
Selecting specific columns:
df[['col1','col2']]

# CONCLUSION:
Data preprocessing is essential for accurate analysis and model performance. Using Python libraries like pandas and sklearn, we can efficiently clean, transform, and prepare data. This experiment demonstrates how raw data can be converted into a structured and meaningful format for further analysis or machine learning tasks.
