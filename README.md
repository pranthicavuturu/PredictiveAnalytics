# Predictive Analysis of Delta Flight Departure Delays

## Running the Notebook on Google Colab
To run the Jupyter Notebook in this repository on Google Colab, follow these steps:

1. Open [Google Colab](https://colab.research.google.com/).
2. Click on `File` > `Open notebook`.
3. Select the `GitHub` tab in the dialog that appears.
4. Enter the URL of this GitHub repository (https://github.com/pranthicavuturu/PredictiveAnalytics) and press `Enter`.
5. Colab will list the notebooks in the repository. Click on the PredictiveAnalyticsProject_Source_Code.ipynb to open.
6. Once the notebook is open in Colab, you can run it by clicking on `Runtime` > `Run all` to execute all cells, or run each cell individually as needed.

The notebook loads the dataset from the GitHub repository. This process will allow you to run the analysis without any local setup requirements, using the computing resources provided by Google Colab. 

## Overview
This project aims to predict flight departure delays for Delta Airlines operating out of Hartsfield-Jackson Atlanta International Airport. By applying predictive analytics techniques, our team seeks to enhance operational efficiency, improve passenger experience, and minimize financial losses caused by flight delays.

## Team Members
- Pranthi Cavuturu
- Muhammad Harris
- Hussain Kaide Johar Manasi

## Problem Statement
Flight delays are a prevalent issue in the airline industry, leading to significant financial losses and decreased customer satisfaction. This project focuses on developing a predictive model to accurately forecast flight delays, thereby assisting Delta Airlines in strategic planning and operational management.

## Objectives
Our goal is to utilize three predictive analytics methods to forecast flight delays:
- **SARIMA**: Leveraged for its effectiveness in understanding seasonal travel trends.
- **LSTM**: Employed to capture complex, nonlinear dependencies within historical delay data.
- **Prophet Model**: Applied for its proficiency in handling daily, weekly, and yearly seasonality, as well as holiday effects.

## Dataset
The analysis is based on approximately 429,000 records from the Bureau of Transportation Statistics, detailing flights from Hartsfield-Jackson Atlanta International Airport during 2022 and 2023. The dataset includes dates, flight details, scheduled and actual departure times, and reasons for delays.

## Methodology
### Data Preprocessing
- Handling missing values through linear interpolation.
- Conversion of date formats and extraction of temporal features.
- Feature scaling using MinMaxScaler and label encoding for categorical features.

### Exploratory Data Analysis
- Analysis of seasonal trends and operational factors influencing delays.

### Predictive Models
1. **SARIMA**
   - Stationarity checked via ADF test.
   - Model selection through Auto ARIMA.
2. **LSTM**
   - Architecture designed to overcome the vanishing gradient problem.
   - Two-layered LSTM with dropout for regularization.
3. **Prophet**
   - Minimal preprocessing required.
   - Seasonality and holiday effects explicitly modeled.

## Results and Evaluation
- **SARIMA**: Achieved a MAE of 2.64 and RMSE of 4.31 on test data.
- **LSTM**: Showed improvement with a MAE of 13.0 and RMSE of 26.78 on test data.
- **Prophet Model**: Best performance post-tuning with a MAE of 2.49 and RMSE of 3.42 on test data.

## Conclusions
The tuned Prophet Model displayed superior predictive performance, making it the most effective for operational planning and customer service enhancements. Our results can significantly impact resource optimization and strategic planning for Delta Airlines.


## Contributions
- **Pranthi Cavuturu**: Worked on on the Prophet Model, exploratory data analysis, and overall project coordination.
- **Muhammad Harris**: Worked on the LSTM model development, data sourcing, and problem statement formulation.
- **Hussain Kaide Johar Manasi**: Worked on the SARIMA model implementation and data preprocessing.
