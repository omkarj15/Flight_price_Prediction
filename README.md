# Flight_price_Prediction

## Introduction

This project focuses on developing a predictive model for flight prices using machine learning techniques. Flight prices are influenced by various factors such as airline, source, destination, departure time, and duration. Therefore, building an accurate predictive model can be beneficial for both airlines and passengers in estimating flight prices.

## Importing Libraries and Dataset

The initial step involves importing essential libraries such as Pandas, NumPy, Matplotlib, Seaborn, Plotly Express, and scikit-learn. Additionally, the training and testing datasets are loaded into the project using Pandas' read_excel() function.

## Feature Engineering

### Basic Exploration

The dataset undergoes basic exploration to understand its structure and characteristics. This includes examining the top 5 records, checking the shape, statistical information, identifying duplicates, and handling missing values.

**Insights:**
- The dataset comprises information about flight prices and related features.
- No duplicate values are found, and only a few missing values are present, which are subsequently removed.

### Data Cleaning

Data cleaning tasks are performed to prepare the dataset for analysis and modeling. This involves removing unnecessary columns, converting time-related features into appropriate formats, and extracting date, month, and year from the 'Date of Journey' column.

**Insights:**
- Columns irrelevant to the model are dropped.
- Time-related features are formatted for better analysis.
- Date, month, and year are extracted for further analysis.

## Exploratory Data Analysis (EDA)

### Preferred Airline

Analysis is conducted to determine the most preferred airline based on the number of flights.

**Insights:**
- Jet Airways emerges as the most preferred airline, capturing 35% of the market share.

### Majority of Flights' Source

The source from which the majority of flights take off is identified.

**Insights:**
- Delhi serves as the primary source for about 42% of flights.

### Maximum Flights Destination

The destination where the maximum number of flights land is determined.

**Insights:**
- Cochin Airport stands out as the most common destination, receiving approximately 42% of flights.

### Impact of Independent Features on Price

The impact of independent features such as airline and additional info on flight prices is analyzed.

**Insights:**
- The airline with the highest price is identified, along with flights priced higher than 50k, especially business class flights.

## Model Building and Evaluation

### Model Selection

Various regression models including Linear Regression, Ridge Regression, Lasso Regression, Decision Tree Regressor, Random Forest Regressor, K-Nearest Neighbors Regressor, Gradient Boosting Regressor, AdaBoost Regressor, and XGBoost Regressor are built and evaluated. Models are assessed based on R-squared score and RMSE on both train and test datasets, with interpretations provided for each model's performance.

### Hyperparameter Tuning

Hyperparameter tuning is performed for Decision Tree, Random Forest, Gradient Boosting, and XGBoost models using GridSearchCV to optimize model performance.

### Model Comparison and Final Selection

Models are compared after hyperparameter tuning, and XGBoost is selected as the final model due to its superior performance on both train and test datasets.

## Prediction on Live Data

### Data Preprocessing

Live data is preprocessed to prepare it for prediction, following similar preprocessing steps as performed on the training data.

### Prediction

The trained XGBoost model is used to predict flight prices on the live data, with predicted prices converted back to their original scale.

### Submission

The final submission dataset containing predicted flight prices is provided.

## Conclusion

The report concludes by summarizing the analysis and highlighting the significance of the predictive model in accurately estimating flight prices. The selection of XGBoost as the final model is justified based on its performance metrics. Suggestions for future improvements or analyses are also provided to enhance the model further.
