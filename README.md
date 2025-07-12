# ComEd Energy Load Forecasting with CNN-LSTM

This project explores electricity consumption forecasting for the ComEd region using a hybrid CNN-LSTM deep learning model. It integrates weather data from multiple stations and applies time-series preprocessing to improve forecast accuracy.

## Files Included

- `notebooks/Final_Project.ipynb`: Main notebook with complete data cleaning, modeling, and evaluation.
- `notebooks/CNN_LSTM.ipynb`, `LSTM.ipynb`, `RNN.ipynb`: Model experiments and comparisons.
- `merged_energy_weather.csv`: Final preprocessed dataset used across models.
- `Final_Project_Report.pdf`: Full write-up including methodology, evaluation, and insights.

## Techniques Used

- Feature Engineering on weather and energy time-series
- CNN for spatial feature extraction
- LSTM for temporal sequence modeling
- SHAP for model interpretability
- Evaluation metrics: RMSE, MAPE

## Libraries

- pandas, numpy, matplotlib, seaborn
- scikit-learn
- PyTorch
- SHAP
- tqdm

## Goal

The aim is to understand how hybrid deep learning models perform on real-world energy datasets and what interpretability tools can reveal about their decisions.

---

Feel free to fork, contribute, or reach out if you’re working on similar problems.
