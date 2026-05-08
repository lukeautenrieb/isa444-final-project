# isa444-final-project
Business forecasting final project comparing statistical, ML, neural, and foundation forecasting models for hotel room demand.

Project Overview

This project forecasts hotel room demand for 17 hotel properties using daily occupancy data. The forecasting horizon was 28 days, and all models were evaluated using 5-fold time-series cross-validation.

The objective was to compare multiple forecasting methods, including baseline models, statistical forecasting models, machine learning forecasting, neural forecasting, and foundation forecasting models.

Models Used:
Baseline Models
Naive
Seasonal Naive
Statistical Models
AutoETS
AutoARIMA
Machine Learning Model
LightGBM (MLForecast)
Neural Forecasting Models
NBEATS
NHITS
Foundation Model
Chronos
Evaluation Metrics

Evaluation metrics used:

Mean Error (ME)
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
Mean Absolute Percentage Error (MAPE)

Model win counts were also calculated to determine which models had the best performance most often.

Main Findings:

The forecasting results showed that hotel occupancy demand has strong weekly seasonality. Seasonal Naive provided a surprisingly competitive benchmark due to the cyclical structure of the data. Statistical models such as AutoETS and AutoARIMA improved forecast smoothness and responsiveness, while the ML model used lags and was able to produce stable occupancy forecasts. Neural forecasting models, specifically NHITS, was most effective at balancing seasonal structure and short-term fluctuations. The foundation model was also pretty strong at predicting demand based on the seasonality of the data, although specialized models often captured the hotel demand more effectively. Therefore, NHITS provided the most accurate forecast model.
