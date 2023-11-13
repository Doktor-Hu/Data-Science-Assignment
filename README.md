# Data Science Assignment - Team Forecasting

**Author:** Zhongyang Hu (zhongyang.hu.rs@gmail.com)

<p align="left">
    <a href="https://en.wikipedia.org/wiki/Autoregressive_integrated_moving_average" title="ARIMA"><img src="https://img.shields.io/badge/Model-ARIMA-blue"></a>
		<a href="https://en.wikipedia.org/wiki/XGBoost" title="XGBoost"><img src="https://img.shields.io/badge/Model-XGBoost-blue"></a>
</p>

<br>

> Please upload the original `sales_data.csv` file yourself in the `../Data` Folder

<br>

> Result csv can be found in the `../RESULT` Folder

---

Introduction: This Jupyter Notebook is for the `Data Science Assignment - Team Forecasting` project. The aim is to create forecasts for the upcoming 12 weeks (not included in the dataset) for all 4 levels.. The datasets used are
- The file `sales_data.csv` with 4 time series of sales at (total, retailer_type_1, retailer_type_2 and retailer_type_3).
- [Brent Crude Oil Futures](https://en.wikipedia.org/wiki/Brent_Crude)
- [COVID-19: Stringency Index](https://ourworldindata.org/explorers/coronavirus-data-explorer?uniformYAxis=0&hideControls=true&Interval=7-day+rolling+average&Relative+to+Population=true&Color+by+test+positivity=false&country=USA~ITA~CAN~DEU~GBR~FRA&Metric=Stringency+index)

The experimented models are:
- ARIMA (a classic statistical model for time-series as a baseline model), and
- XGBoost (a prevalently used machine learning model)

After experiments and validation, I decided to use the XGBoost model for the final forecast.

More overviews can be viewed by clicking the > below.

---

<br>

### Notebook Environments

_Developed originally using Google CoLab._

<br>

### Notebook Structure

<details><summary>click here to check details</summary>


Part I: Preparation and Data Exploration

- Section 1: Prepare Environment and Setups

- Section 2: Basic Overview of the Dataframe

- Section 3: Training/Validation/Testing Dataset Split

- Section 4: Time-Series Analysis

Part II: Modelling and Validation

- Section 5: Baseline Model: ARIMA

- Section 6: XGBoost Model: Experiments

Part III: Forecasting

- Section 7: Model Selection and Final Forecasting

</details>

<br>

### Key Take-away Messages

<details><summary>click here to check details</summary>

- ARIMA models tend to converge towards a constant, leading to a reduced ability to capture variations effectively.

- Underfitting is observed in XGBoost, and its behavior varies between single-point prediction and recurrent forecasting.

- A noticeable distribution shift has been identified across the training, validation, and testing datasets, resulting in a conceptual shift within the model.

- The presence of anomalies in `retailer_type_3` during the year 2020 adds complexity to the forecasting task, warranting heightened attention.

</details>

<br>
