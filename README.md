# Fuel Economy Data Analysis

## Overview

This repository contains an R script for analyzing the fuel economy data using the `mpg` dataset from the `ggplot2` package. The analysis involves preprocessing techniques, fitting a Generalized Linear Model (GLM) using H2O in R, and evaluating the model's performance.

## Script Details

### 1. Data Exploration

- **Libraries:** The script utilizes various R libraries for data manipulation, visualization, and modeling, including `tidyverse`, `data.table`, `skimr`, `inspectdf`, `mice`, `plotly`, `recipes`, `caret`, `h2o`, and others.

- **Data Loading:** The `mpg` dataset from `ggplot2` is loaded for analysis.

- **Data Exploration:** The script explores the data using `skimr` for summary statistics and `inspect_na` for identifying missing values.

- **Outlier Handling:** Outliers in numeric variables are identified and handled, with a focus on the 'cty' variable.

### 2. Modeling

- **Linear Regression with H2O:** A GLM is fitted using the H2O library in R. The modeling structure is specified as `cty ~ year + cyl + displ`.

- **Multicollinearity Check:** The script checks and handles multicollinearity using Variance Inflation Factor (VIF).

- **Model Training and Evaluation:** The data is prepared, standardized, and split into training and testing sets. The H2O GLM model is built and evaluated on various metrics.

- **Model Summary:** Coefficients table with p-values is printed, providing insights into the significance of predictors.

### 3. Evaluation

- **Performance Metrics:** The script calculates and displays metrics such as Root Mean Squared Error (RMSE), R-squared, and Adjusted R-squared for both the test and training sets.

- **Visualization:** The results are visualized using ggplot2 and converted to interactive plots using plotly.

### 4. File Naming

- The final R script is named as "Fuel_Economy_Data_Analysis.R".

## Usage

To replicate the analysis:

1. Ensure you have R and the required libraries installed.
2. Run the script in an R environment, considering any specific package dependencies.

## Author

- **Ilaha Musayeva**
- **Date: 10.25.2023**


