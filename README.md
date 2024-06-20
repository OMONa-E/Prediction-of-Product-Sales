# Prediction of Product Sales

## Project Overview

This project aims to predict product sales using a dataset provided by Omona Emmanuel. The dataset contains information about various products and their sales across different outlets. The project involves data cleaning, preprocessing, and exploratory data analysis (EDA) to gain insights into the dataset before building predictive models.

## File Description

- `Prediction_of_Product_Sales.ipynb`: Jupyter Notebook containing the Python code for data cleaning, preprocessing, and EDA.
- `sales_predictions_2023.csv`: Dataset file containing the raw data used in the analysis.
- `ML_model_for_product_sales_prediction.ipynb`: Jupyter Notebook containing the Python code for Machine Learning model

## Dependencies

- pandas
- numpy
- missingno
- seaborn
- matplotlib
- sklearn
- Google Colab (for notebook execution and visualization)

## Data Exploratory Data Analysis (EDA)

The exploratory data analysis (EDA) section of the project involves:

- **Checking Data Distribution:** Histograms are used to visualize the distribution of numerical features in the dataset.
  ![Histograms for Numerical Features](https://github.com/OMONa-E/Prediction-of-Product-Sales/blob/main/Histograms%20Numerical%20Feature.png)
  
- **Summary Statistics:** Boxplots provide statistical summaries of numerical features, such as median, quartiles, and outliers.
- **Frequency Analysis:** Countplots are utilized to analyze the frequency of each class in categorical features.
  
- **Correlation Analysis:** A heatmap is used to visualize the correlation between features in the dataset.
  ![Histograms for Numerical Features](https://github.com/OMONa-E/Prediction-of-Product-Sales/blob/main/Correlation%20Heatmap.png)

The EDA process helps in understanding the underlying patterns, relationships, and characteristics of the data, which is crucial for building accurate predictive models.

# ML Model for Prediction of Product Sales

## Overview of the Project
This project focuses on developing machine learning models to predict product sales based on various product and outlet attributes. The primary objective is to assist retailers in understanding the factors influencing sales and optimizing inventory management and marketing strategies.

## Relevant Insights from the Data
1. **Correlation Analysis:** Visualizing the correlation matrix revealed that the "Item MRP" feature has a strong positive correlation with "Item Outlet Sales," indicating that higher maximum retail prices tend to result in higher sales figures.

2. **Categorical Feature Analysis:** Investigating the distribution of categorical features, such as "Item Fat Content," uncovered inconsistencies that were addressed during data cleaning. This step ensured the reliability of the dataset for model training.

## Summary of the Model and Evaluation Metrics
- **Linear Regression Model:** Demonstrates slight underfitting, with consistent performance between training and test datasets. Achieves an R-squared value of 0.587 and an RMSE of 1067.926 units on the test dataset.
- **Random Forest Model:** Exhibits clear signs of overfitting, with significantly better performance on the training data than on the test data. Achieves an R-squared value of 0.882 and an RMSE of 662.983 units on the training dataset, indicating potential overfitting issues.

## Final Recommendations
While the Linear Regression model demonstrates better generalization to unseen data, the Random Forest model suffers from overfitting and may require further optimization or regularization techniques to improve its performance on test data. It's recommended to explore techniques such as hyperparameter tuning and feature engineering to enhance model performance and address overfitting concerns.

## Usage

To run the notebook locally, ensure you have Python installed along with the required dependencies listed above. Then, execute the cells in the Jupyter Notebook sequentially to perform data cleaning, preprocessing, and exploratory data analysis.

## Credits

- **Author:** Omona Emmanuel
- **Project Completion Date:** Apr 10, 2024

## License

This project is licensed under the [MIT License](LICENSE).
