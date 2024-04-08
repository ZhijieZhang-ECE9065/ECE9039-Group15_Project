# Store Sales Forecasting Project

## Abstract

This project focuses on forecasting store sales for a major grocery retailer in Ecuador, utilizing a rich dataset that spans from January 1, 2013, to August 15, 2017. The dataset encompasses sales information across 54 stores and 33 product families, providing a detailed view of historical sales trends and patterns. Our analysis aims to predict future sales across various stores and product families, and to leverage these forecasts in providing actionable restocking recommendations.

## Dataset Overview

The analysis utilizes six distinct datasets: “train”, “test”, “store”, “transactions”, “holidays_events”, and “oil”. A notable challenge encountered was the absence of actual sales data in the "test" dataset. This limitation led us to extract a portion of the "train" dataset to serve as a new testing set, ensuring the reliability of our model evaluation process.

### Data Preprocessing

Key steps in our data preprocessing phase included:
- Loading essential datasets: "Sales.csv", "holidays_events.csv", "stores.csv", "oil.csv", and "transactions.csv".
- Converting date columns into datetime format to facilitate time series analysis.
- Transforming data types for efficient processing and applying one-hot encoding on categorical features for machine learning readiness.
- Aggregating transaction data monthly and merging it with store information to enrich the feature set.
- Splitting the data: 80% for training and the remaining 20% as the test set, followed by thorough data cleaning to enhance data quality.

### Exploratory Data Analysis (EDA)

Our EDA phase involved generating several visualizations to understand sales and transaction trends, including:
- Transaction volumes by year and month.
- Average monthly transactions and daily sales performance.
- Popularity of product categories among customers.
- Sales trends across different cities.

### Time Series Forecasting

For forecasting store sales, we employed time series analysis to capture seasonal patterns and temporal dependencies. The LightGBM model was chosen for its efficiency and ability to handle the dataset's complexity, supported by a rigorous hyperparameter tuning process.

### Model Training and Output

The model training phase underscored the selection of optimal hyperparameters and the utilization of the LightGBM model, demonstrating its capability to predict future sales with a reasonable degree of accuracy. Performance metrics such as RMSE and MAE were employed to evaluate the model's effectiveness.

### Prophet Model for Transactions and Sales Prediction

We also utilized the Prophet model for predicting future sales trends and transactions, focusing on long-term trends crucial for strategic inventory management.

## Conclusion

Our project illustrates the potential of advanced forecasting models in enhancing operational efficiency and customer satisfaction, providing valuable insights for competitive market positioning.

## Acknowledgments

We express our sincere gratitude to our instructor, Soodeh Nikan, for her expert guidance and support throughout this project. Her invaluable advice was instrumental to our success.

## References

1. "Store Sales - Time Series Forecasting," Kaggle. [https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data](https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data)
