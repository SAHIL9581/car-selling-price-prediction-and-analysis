# Car Price Prediction

A machine learning project to predict the selling price of used cars based on various features like age, present price, kilometers driven, fuel type, and more.

## Overview

This project analyzes a dataset of used car sales to build a prediction model for estimating car selling prices. The model leverages Linear Regression to find relationships between car features and their market values.

## Dataset

The dataset contains information about used cars with the following features:
- Car_Name: Name of the car model
- Year: Year of manufacture
- Selling_Price: Price at which the car was sold (target variable)
- Present_Price: Current market price of the car
- Kms_Driven: Total kilometers driven
- Fuel_Type: Type of fuel (Petrol, Diesel)
- Seller_Type: Type of seller (Dealer, Individual)
- Transmission: Transmission type (Manual, Automatic)
- Owner: Number of previous owners

## Exploratory Data Analysis

The project includes comprehensive EDA with visualizations:
- Distribution of car manufacturing years
- Selling price distributions by transmission type
- Distribution of kilometers driven
- Correlation analysis between numerical features
- Scatter plots showing relationships between key features and selling price

## Model Building

The model development process includes:
1. Data preprocessing with one-hot encoding for categorical features
2. Train-test splitting (70-30 ratio)
3. Feature standardization using StandardScaler
4. Linear Regression model training and evaluation

## Model Performance

Performance metrics of the Linear Regression model:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE) on test data
- Mean Squared Error (MSE) on training data
- R² score

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- plotly

## Usage

```python
# Example of model prediction
# Load the model
# model = load_model('car_price_model.pkl')

# Input new car data
new_car = [[2015, 8.5, 30000, 0, True, False, False, True]]  # Example values
# Remember to preprocess and scale the input

# Get prediction
# predicted_price = model.predict(new_car)
# print(f"Predicted selling price: ${predicted_price[0]:.2f}")
```

## Key Findings

- Present price (current market value) has a strong positive correlation with selling price
- Car age negatively impacts selling price
- Kilometers driven has a slight negative correlation with selling price
- The linear regression model captures these relationships effectively

## Future Improvements

- Implement more complex models like Random Forest or XGBoost
- Feature engineering to create more predictive variables
- Hyperparameter tuning for better model performance
- Web interface for easy predictions

## License

[MIT](https://choosealicense.com/licenses/mit/)
