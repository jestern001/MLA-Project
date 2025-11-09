Things to try
- A non-linear model
    - LightGBM
- A forecasting model
    - issues
        1) Temporal independence: You are primarily interested in the nighttime NO2​ value based on the preceding day's conditions, treating each day-night cycle as an independent event.
        2) Missing Data: If you only have daily TEMPO snapshots, you don't have the continuous data needed to train a robust LSTM or ARIMA model effectively.
        3) Efficiency: Forecasting models are computationally intensive and would be less "light" than the recommended LightGBM regression approach.
        - Ref: https://arxiv.org/html/2501.06907v1


