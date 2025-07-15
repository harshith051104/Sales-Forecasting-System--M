# Sales Forecasting System

This project uses an ARIMA (AutoRegressive Integrated Moving Average) model to forecast sales based on historical data.

## Dataset

The project uses a synthetically generated dataset representing daily sales data from January 1, 2022, to December 31, 2024. The data is created to simulate a realistic sales pattern, including a trend, seasonality, and random noise.

## Model

An **ARIMA** model is used for this time series forecasting task. The model is trained on 90% of the dataset and tested on the remaining 10%. The model is configured with the following order `(p, d, q)`:

* **p=5**: The number of lag observations included in the model (lag order).
* **d=1**: The number of times that the raw observations are differenced (degree of differencing).
* **q=0**: The size of the moving average window (order of moving average).

## Libraries Used

* Pandas
* Numpy
* Statsmodels
* Scikit-learn
* Matplotlib

## How to Run

1.  Clone the repository:
    ```
    git clone [https://github.com/your-username/sales-forecasting-system.git](https://github.com/your-username/sales-forecasting-system.git)
    ```
2.  Install the required libraries:
    ```
    pip install pandas numpy statsmodels scikit-learn matplotlib
    ```
3.  Run the Jupyter Notebook:
    ```
    jupyter notebook forecasting.ipynb
    ```

## Results

The model's performance was evaluated using two key metrics:

* **Root Mean Squared Error (RMSE):** 17.72
* **Mean Absolute Percentage Error (MAPE):** 7.60%

### Sales Forecast vs. Actual Data

The plot below visualizes the model's forecasts against the actual sales data on the test set, showing the training data, the actual test data, and the forecasted sales.

<img width="1005" height="624" alt="image" src="https://github.com/user-attachments/assets/7526a63f-0bab-479a-b289-e1f50335364f" />
