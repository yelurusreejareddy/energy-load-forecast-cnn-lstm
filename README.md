# energy-load-forecast-cnn-lstm

Hourly electricity demand prediction for the Illinois ComEd service area using
a hybrid CNN-LSTM deep learning model with SHAP interpretability.

## Files Included

- energy_load_forecast_cnn_lstm.ipynb - main notebook with full pipeline and SHAP analysis
- cnn_lstm_model.ipynb - CNN-LSTM model experiments
- lstm_baseline.ipynb - LSTM baseline comparison
- rnn_baseline.ipynb - RNN baseline comparison
- merged_energy_weather.csv - merged ComEd hourly load and weather data
- project_report.pdf - full write-up with methodology, evaluation, and insights

## Techniques Used

- Dataset built by parsing ComEd service area locations and merging with hourly weather data
- Feature engineering on weather and energy time-series
- CNN for local pattern extraction across time windows
- LSTM for temporal sequence modeling
- CNN-LSTM hybrid combining both for improved accuracy
- SHAP values to identify which weather and time features drove predictions most
- Evaluation metrics: RMSE, MAPE

## Libraries

pandas, numpy, matplotlib, seaborn, scikit-learn, PyTorch, SHAP, tqdm

## Goal

To predict hourly electricity load for the ComEd Illinois service area and explain
model decisions using SHAP, comparing deep learning architectures on the same data.
