## UK House Price Index – Forecasting Over Time

## Overview  
This project looks at and predicts the UK House Price Index (UK HPI) using traditional time series methods.  
The aim is to compare different ways of making predictions and see how well they work.

The models I used are:  
- ARIMA (a standard model)  
- ARIMAX (which includes extra factors)  
- ETS / Holt–Winters (with a 95% confidence range for predictions)

This project is part of a university MSc Data Science course. It shows how to develop models in a controlled way using GitHub and Google Colab.

---

## Dataset  
I used the official UK House Price Index dataset from HM Land Registry.

Because the file is too big, the original data isn't in this repository.

Dataset source:  
https://www.gov.uk/government/statistical-data-sets/uk-house-price-index-data-downloads-july-2025?utm_source=chatgpt.com#download-the-data

---

## Methodology
The analysis is done in the following steps:
- Loading and cleaning the data
- Exploratory Data Analysis (EDA)
- Creating a monthly UK-wide house price time series
- Applying a log transformation and splitting the data into training and testing sets (24 months ahead)
- Checking if the data is stationary using the Augmented Dickey–Fuller test
- Building models:ARIMA, ARIMAX (with extra variables),ETS (Holt–Winters)
- Evaluating forecasts with:RMSE, MAE, MAPE
- Estimating forecast uncertainty using 95% confidence intervals


---


## Key Findings
- ARIMAX performed the best overall, showing how useful extra information can be.
- ETS gave smooth predictions with clear seasonal patterns and easy-to-understand uncertainty ranges.
- ARIMA was a solid baseline, but didn’t do as well when more data was available.

---

## How to Run the Notebook
- Open the file uk_hpi_Dec.ipynb in Google Colab.
- Upload or connect to the UK HPI dataset.
- Run each cell one after the other, starting from the top.
- The plots and results will be saved automatically in the results_dissertation folder.

---
