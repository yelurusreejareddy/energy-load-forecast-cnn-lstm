# energy-load-forecast-cnn-lstm

Team project predicting hourly electricity demand for the Illinois ComEd service area
with a hybrid CNN-LSTM deep learning model, compared against LSTM and RNN baselines.

## Files Included

- energy_load_forecast_cnn_lstm.ipynb - main notebook with the full pipeline
- cnn_lstm_model.ipynb - CNN-LSTM model experiments
- lstm_baseline.ipynb - LSTM baseline comparison
- rnn_baseline.ipynb - RNN baseline comparison
- merged_energy_weather.csv - merged ComEd hourly load and weather data
- project_report.pdf - full write-up with methodology, evaluation, and insights

## Techniques Used

- Dataset built by merging 66k hourly ComEd load readings with weather data from 17 regional stations
- Feature engineering on weather and energy time series, using 24-hour input windows
- 1D convolution for local pattern extraction within each window
- 3-layer LSTM for temporal sequence modeling
- Evaluation metrics: RMSE and MAPE

## Results

| Model | MAPE | RMSE |
|---|---|---|
| CNN-LSTM | 1.40% | 205.76 MW |
| LSTM baseline | 3.37% | 523.51 MW |
| RNN baseline | 7.14% | 1024.45 MW |

## Libraries

pandas, numpy, matplotlib, seaborn, scikit-learn, PyTorch, tqdm

## Goal

To predict hourly electricity load for the ComEd Illinois service area and compare
deep learning architectures on the same data.
