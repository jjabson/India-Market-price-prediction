# India Used Car Price Prediction

## Project Overview

This project develops a machine learning solution to predict the resale price of used cars in the Indian automotive market. The objective is to help buyers, sellers, dealerships, and automotive platforms estimate fair market value using vehicle characteristics, ownership history, and usage patterns.

The project follows a complete end-to-end machine learning workflow, including:

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering
* Model development and evaluation
* Error analysis and business interpretation

---

## Business Problem

Pricing used vehicles accurately is challenging because vehicle value depends on multiple factors such as:

* Vehicle age
* Brand and model
* Mileage
* Engine size
* Power output
* Fuel type
* Transmission type
* Ownership history
* Vehicle usage

Traditional pricing methods often rely on manual estimates and market experience. This project demonstrates how machine learning can provide a more consistent and data-driven valuation process.

---

## Dataset

The dataset contains used vehicle listings from the Indian automobile market.

### Features

* Name
* Location
* Year
* Kilometers_Driven
* Fuel_Type
* Transmission
* Owner_Type
* Mileage
* Engine
* Power
* Seats
* New_price
* Price (Target Variable)

### Target

* **Price** – Used car selling price

---

## Project Workflow

### 1. Data Understanding

Performed initial inspection of:

* Dataset dimensions
* Data types
* Missing values
* Duplicate records
* Summary statistics

### 2. Data Cleaning

Key preprocessing steps included:

* Removing identifier columns
* Handling missing values
* Converting data types
* Treating invalid values
* Addressing outliers
* Cleaning categorical variables

### 3. Feature Engineering

Created additional business-relevant features such as:

* Car Age
* Kilometers Driven per Year
* Vehicle Brand
* Capped mileage-related outliers

These engineered features improved the model's ability to capture vehicle depreciation patterns.

### 4. Exploratory Data Analysis

Explored:

* Price distribution
* Vehicle age distribution
* Mileage trends
* Brand-level pricing differences
* Correlations among numerical variables
* Outlier behavior

### 5. Model Development

Built regression models to predict vehicle price.

Models evaluated include:

* Linear Regression
* Ridge Regression
* Additional regularized approaches

The objective was to balance:

* Predictive performance
* Model interpretability
* Generalization to unseen vehicles

### 6. Model Evaluation

Performance was assessed using regression metrics such as:

* MAE (Mean Absolute Error)
* RMSE (Root Mean Squared Error)
* MAPE (Mean Absolute Percentage Error)
* R² Score

Visual evaluation included:

* Actual vs Predicted Price plots
* Residual analysis
* Error distribution analysis

---

## Key Findings

### Vehicle Age Matters

Older vehicles generally experience significant depreciation, making age one of the strongest predictors of resale value.

### Premium Brands Retain Value Better

Luxury and premium brands tend to maintain higher resale prices compared to economy vehicles.

### Mileage Has Strong Impact

Higher mileage is associated with lower resale value due to increased wear and tear.

### Engine and Power Influence Pricing

Vehicles with larger engines and higher power outputs generally command higher prices.

### Feature Engineering Improved Performance

Derived variables such as vehicle age and usage intensity improved predictive capability beyond raw features alone.

---

## Results

The final model successfully learned pricing patterns across thousands of used vehicles and demonstrated strong predictive performance on unseen data.

The model can be used as a decision-support tool for:

* Used car dealerships
* Online automotive marketplaces
* Vehicle valuation services
* Individual buyers and sellers

---
## Model Performance

The final regression model was evaluated using standard regression metrics:

| Metric | Value |
|---|---:|
| MAE | 1.214 |
| RMSE | 2.753 |
| MAPE | ~12% |
| R² Score | 0.938 |

The model was also evaluated visually using actual vs predicted plots, residual analysis, and prediction error plots.

![Actual vs Predicted](images/actual_vs_predicted.png)

![Residual Plot](images/residual_plot.png)

## Technologies Used

### Programming Language

* Python

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib
* Seaborn

### Machine Learning

* Scikit-Learn

### Development Environment

* Jupyter Notebook
* Google Colab

---

## Repository Structure

```text
india-used-car-price-prediction/
│
├── notebooks/
│   └── India_Used_Car_Price_Prediction.ipynb
│
├── data/
│   └── used_cars.csv
│
├── images/
│   ├── price_distribution.png
│   ├── residual_plot.png
│   └── actual_vs_predicted.png
│
├── requirements.txt
│
└── README.md
```

---

## Future Improvements

Potential enhancements include:

* Gradient Boosting Models (XGBoost, LightGBM, CatBoost)
* Hyperparameter optimization
* Ensemble models
* Feature selection techniques
* Model deployment using Flask/FastAPI
* Real-time vehicle valuation application

---

## Business Impact

Accurate used car pricing is important for both buyers and sellers because vehicle resale value can vary significantly based on age, mileage, brand, fuel type, transmission, ownership history, and vehicle specifications. This project demonstrates how machine learning can support a more consistent and data-driven pricing process in the used car market.

### How this solution can help

- **Dealership pricing support:** Dealerships can use the model to estimate fair listing prices and reduce reliance on manual judgment alone.
- **Buyer decision support:** Buyers can compare a listed price against a model-estimated fair value to identify potentially overpriced or underpriced vehicles.
- **Seller price guidance:** Individual sellers can use predicted prices to set more competitive asking prices.
- **Marketplace valuation:** Online automotive platforms can integrate a model like this into price recommendation tools for listings.
- **Inventory strategy:** Businesses can analyze pricing trends by brand, age, mileage, and vehicle type to make better purchase and resale decisions.

### Business value

By combining vehicle attributes with historical market pricing patterns, the model can help reduce pricing inconsistency, improve transparency, and support faster decision-making. While the model should not replace expert appraisal or real-time market research, it can serve as a useful decision-support tool for estimating used car resale value.

---

## Conclusion

This project demonstrates a complete machine learning pipeline for solving a real-world regression problem. By combining domain knowledge, feature engineering, and predictive modeling, the solution provides a practical framework for estimating used car prices in the Indian market.

The project highlights how data-driven approaches can improve pricing accuracy and support better decision-making within the automotive industry.

## Author: Jerome Jabson

