# Diamond Price Prediction using Random Forest Regression

This R script performs diamond price prediction using a random forest regression model. It includes data preprocessing, feature engineering, model fitting, and evaluation.

## Overview

The script performs the following tasks:

1. **Data Preprocessing:** Loads the diamonds dataset from the `tidyverse` package, adds a group ID and its size, and calculates the log of the price as the target variable.

2. **Duplicate Detection:** Identifies duplicate records in the dataset and calculates the proportion of duplicates.

3. **Model Fitting:** Fits a random forest regression model using the `ranger` package, considering carat, cut, color, and clarity as predictor variables.

4. **Cross-Validation:** Performs 5-fold cross-validation using different split types (basic and grouped) and evaluates the model's performance using root mean squared error (RMSE).

## Libraries Used

The script utilizes the following R packages:

- `tidyverse`: For data manipulation and visualization.
- `ranger`: For fitting random forest regression models.
- `splitTools`: For creating folds for cross-validation.

## Usage

To use the script:

1. Install the required packages by running the following commands in R:

   ```r
   install.packages("tidyverse")
   install.packages("ranger")
   install.packages("splitTools")
