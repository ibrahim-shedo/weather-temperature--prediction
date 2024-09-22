# Weather Data Analysis with Simple Linear Regression

## Overview
This project analyzes a weather dataset to predict air temperature (`Temp_C`) using the dew point temperature (`Dew_Point_Temp_C`) as a feature. The goal is to build a simple linear regression model that provides insights into how dew point temperature influences air temperature.

## Dataset Variables
- **Date/Time**: Timestamp of the weather observation.
- **Temp_C**: Air temperature in degrees Celsius (target variable).
- **Dew_Point_Temp_C**: Temperature at which air becomes saturated with moisture (feature variable).
- **Rel Hum_%**: Relative humidity percentage.
- **Wind Speed_km/h**: Wind speed in kilometers per hour.
- **Visibility_km**: Distance that can be clearly seen in kilometers.
- **Press_kPa**: Atmospheric pressure in kilopascals.
- **Weather**: Description of weather conditions (e.g., sunny, rainy).

## Feature Selection
For this analysis, the following features will be used:
- **Feature Variable**: `Dew_Point_Temp_C`
- **Target Variable**: `Temp_C`

## Methodology
1. **Data Preprocessing**:
   - Load the dataset using pandas.
   - Check for and handle missing values.
   - Convert data types if necessary (e.g., ensuring temperature fields are numeric).

2. **Feature Selection**:
   - Select `Dew_Point_Temp_C` as the independent variable (X) and `Temp_C` as the dependent variable (y).

3. **Splitting the Data**:
   - Split the dataset into training and testing sets using `train_test_split` from scikit-learn.

4. **Model Training**:
   - Import the `LinearRegression` class from scikit-learn.
   - Create an instance of the linear regression model.
   - Fit the model using the training data (`X_train` and `y_train`).

5. **Model Evaluation**:
   - Make predictions using the test set (`y_pred`).
   - Evaluate the model's performance using metrics such as R-squared and Mean Squared Error (MSE).

6. **Visualization (Optional)**:
   - Plot the regression line against the data points to visualize the relationship between `Dew_Point_Temp_C` and `Temp_C`.

## Requirements
- Python 3.x
- pandas
- scikit-learn
- matplotlib (for visualization, if needed)

## Usage
1. Clone the repository:
   ```bash
   git clone [repository-url]
   cd [repository-folder]
Install the required packages:

bash
Copy code
pip install pandas scikit-learn matplotlib
Run the analysis script:

bash
Copy code
python weather_analysis.py
Conclusion
This analysis aims to provide insights into the relationship between dew point temperature and air temperature, which can be valuable for understanding weather patterns.
