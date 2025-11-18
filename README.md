# Walmart Weekly Sales Forecasting with Chronos
Project Overview
This project focuses on forecasting weekly sales for various Walmart stores using the advanced Chronos deep learning model. The goal is to provide accurate 4-week ahead sales predictions to assist with operational planning, inventory management, and strategic decision making within the retail environment. We employ robust data preprocessing techniques and thorough performance evaluation to assess the model's efficacy.

Features & Highlights
Data Loading & Preprocessing: Efficient loading of historical Walmart sales data, including handling outliers and converting daily sales into a weekly time series format.
Log Transformation: Application of a log transformation (np.log1p) to weekly sales data, a crucial step for optimizing Chronos model performance by stabilizing variance.
Chronos Model Integration: Utilization of the amazon/chronos-t5-tiny pre trained model for state of the art time series forecasting.
4-Week Ahead Forecasts: Generation of weekly sales predictions for the next four weeks, complete with 90% confidence intervals to quantify uncertainty.
Comprehensive Performance Evaluation: Rigorous assessment of forecast accuracy using key metrics: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE).
Visualizations: Clear plots illustrating actual weekly sales against forecasted values and their confidence intervals for each store.
Key Insights & Achievements
The Chronos model demonstrates significant potential for retail sales forecasting. While performance varies across stores, it achieved exceptional accuracy for specific locations:

High Accuracy for Specific Stores: Notably, Store 30 exhibited a remarkable MAPE of 1.91%, and Store 33 achieved an even lower MAPE of 1.70%. This indicates that for stores with more consistent or predictable sales patterns, the Chronos model delivers highly reliable forecasts (deviating by less than 2% on average).
Varied Performance: The evaluation highlights that some stores are more challenging to predict, with higher error rates.

Technologies Used
Python
Pandas (for data manipulation)
NumPy (for numerical operations)
Chronos (Deep Learning Forecasting Library)
Scikit-learn (for evaluation metrics)
Matplotlib & Seaborn (for visualizations)
Holidays (for holiday marking on plots)
