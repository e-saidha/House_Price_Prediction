🏠 House Price Prediction using XGBoost

A complete machine learning regression project to predict California house prices using the California Housing dataset.
This notebook walks through data exploration, visualization, model training, hyperparameter tuning, and real-time prediction — all in Google Colab.

📘 Project Overview

The goal of this project is to predict the median value of houses in California districts based on demographic and geographic features such as:

Median income

Average number of rooms and bedrooms

Population and occupancy

Latitude and longitude

Project Workflow

Data Loading & Cleaning – Import the dataset using fetch_california_housing from sklearn.datasets.

Exploratory Data Analysis (EDA) – Understand data distribution and correlations between features.

Visualization – Plot a correlation heatmap to identify key drivers of house prices.

Model Building – Train an XGBoost Regressor to capture nonlinear relationships.

Model Evaluation – Assess performance using R² score and Mean Absolute Error (MAE).

Hyperparameter Tuning – Optimize model using RandomizedSearchCV.

Predictions – Predict house prices for new unseen input data.

📊 Model Performance
Metric	Training Set	Test Set
R² Score	~0.83	~0.82
Mean Absolute Error (MAE)	~0.31	~0.32

✅ The tuned XGBoost model achieves strong and stable performance, generalizing well across unseen data.

🔍 Sample Prediction

Input Example:

{
  'MedInc': 3.8,
  'HouseAge': 28.6,
  'AveRooms': 5.4,
  'AveBedrms': 1,
  'Population': 2000,
  'AveOccup': 3,
  'Latitude': 34.5,
  'Longitude': -119.2
}


Predicted Median House Value: ≈ 2.1 ($100,000 units)

🧠 Tools & Libraries

Python 3

Pandas, NumPy – Data analysis

Matplotlib, Seaborn – Visualization

Scikit-learn – Model evaluation and tuning

XGBoost – Gradient boosting regression model

Google Colab – Development environment

📂 Repository Structure
File	Description
house_price_prediction.ipynb	Main notebook containing full workflow – EDA, training, tuning, and prediction
README.md	Project overview and documentation
💡 Key Learnings

How to train and evaluate a regression model using XGBoost

Understanding feature correlations and their impact on predictions

Applying hyperparameter tuning to improve model performance

Making predictions on new custom input data

🚀 Future Improvements

Add feature importance visualization

Compare performance with Linear Regression and Random Forest

Deploy as an interactive Streamlit app
