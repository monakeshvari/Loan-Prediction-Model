# # Loan Prediction Model

This project is focused on predicting the loan amount based on various features using different regression techniques. The dataset used for this project contains information about loans, such as loan type, repayment status, start and end dates, and interest rates.

## Dataset
loans.csv: https://drive.google.com/file/d/1fvDocGh8U6RCZHrF4pMdnGkqmPr12rCH/view?usp=drive_link


## Project Overview

### 1. Data Loading

The dataset is read from a CSV file located in Google Drive.

### 2. Dataset Exploration

- **Initial Data Inspection**: Displaying the first few rows, checking the shape and data types of the dataset.
- **Missing Values**: Checking for and handling missing values.
- **Statistical Summary**: Providing descriptive statistics for numerical columns.
- **Duplicate Rows**: Checking for and handling duplicate rows.
- **Unique Values**: Displaying unique values for categorical columns.
- **Dataset Information**: Providing a concise summary of the DataFrame.

### 3. Data Visualization

- **Value Counts Visualization**: Visualizing the distribution of values in categorical columns using bar plots and pie charts.

### 4. Data Preprocessing

- **Handling Duplicates**: Removing any duplicate rows.
- **Dropping Unnecessary Columns**: Removing columns that are not needed for analysis.
- **Handling Missing Values**: Imputing missing values using the most frequent value for categorical columns and the mean for numerical columns.
- **Date Type Conversion**: Converting date columns from object to datetime and then to timestamp.
- **Outliers Handling**: Detecting and handling outliers using the Interquartile Range (IQR) method.

### 5. Data Transformation

- **Label Encoding**: Encoding categorical variables into numerical values.
- **Data Transformation**: Applying various transformations (Square Root, Logarithm, Reciprocal, Box-Cox) to reduce skewness in numerical columns.

### 6. Feature Engineering

- **Standardization**: Standardizing numerical features to have zero mean and unit variance.
- **Correlation Matrix**: Visualizing the correlation between different features.
- **Polynomial Features**: Creating polynomial features of degree 2 and 3 for more complex models.

### 7. Data Splitting

- **Train-Test Split**: Splitting the data into training and testing sets for different models: Simple Linear Regression (SLR), Multiple Linear Regression (MLR), and Polynomial Regression (degree 2 and 3).

### 8. Modeling and Prediction

- **Model Training**: Training different regression models (SLR, MLR, Polynomial degree 2, and Polynomial degree 3).
- **Prediction**: Making predictions on the test data using the trained models.

### 9. Model Evaluation

- **Evaluation Metrics**: Calculating evaluation metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R2) for each model.
- **Model Comparison**: Comparing the models based on the evaluation metrics to determine the best performing model.

### 10. Results

- The best model based on the lowest MAE and MSE, as well as the highest R2, is identified as the Polynomial Regression model with degree 3 (POL3).
