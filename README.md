# AI/ML Project: Forecasting Air Passengers ✈️

<p align="center"><img src="https://user-images.githubusercontent.com/54996245/142404359-8c4e3e8b-b791-4bde-b8d0-6bfb979ff2b6.png" style="width: 1000px;"/></p>

### Description:

A simple yet challenging project, to forecast the volume of air passengers, based on monthly totals of a US airline passengers from 1949 to 1960.
Can you overcome the obstacles & Forecast the future occupancies of the Airlines?

**This data frame contains the following columns:**

* Month : The month of observation
* #Passengers : Total Passengers travelled in that particular month

**Source:**

This dataset is taken from an inbuilt dataset of R called AirPassengers.<br>
Kaggle - 
https://www.kaggle.com/yersever/500-person-gender-height-weight-bodymassindex


### Objectives:
- Understand the Dataset & cleanup (if required).
- Perform the necessary checks like stationarity & DF on the Dataset.
- Build a forcasting model to predict the future volumne of the air passengers.

### The Project is divided into the following steps:
1. Visualize the time series - Check for trend, seasonality, or random patterns.
2. Stationarize the series using decomposition or differencing techniques.
3. Plot ACF/PACF and find (p,d,q) parameters.
4. Building the forecasting model - can be AR, MA, ARMA or ARIMA.
5. Making Predictions using the Forecasting Model

### Some Visuals of the Project:

**1. Time-Series Data**
<p align="left"><img src="https://user-images.githubusercontent.com/54996245/142403596-7d80968c-45fa-4608-a04c-4549495e5369.png" /></p>

**2. Stationarity Check**

![image](https://user-images.githubusercontent.com/54996245/142403752-886b1fe4-d367-458e-808d-ac788e368ec6.png)

**3. Decomposing using moving average**

![image](https://user-images.githubusercontent.com/54996245/142403822-0ed25762-a68f-4ee7-be1f-200b4f21c1fc.png)

**4. Stationarity Check for Decomposed data**

![image](https://user-images.githubusercontent.com/54996245/142403896-46f6065b-6646-4d8a-9685-f827228bd173.png)

**5. Auto Correlation Function Plot**

![image](https://user-images.githubusercontent.com/54996245/142403996-65048935-bde5-4f8b-b4c3-24703ab3ff9e.png)

**6. Partial Auto Correlation Function Plot**

![image](https://user-images.githubusercontent.com/54996245/142404090-92d30d4f-f800-4a94-a59b-09148e581435.png)

**7. ARIMA Model Forecast**

![image](https://user-images.githubusercontent.com/54996245/142404128-59c19a3c-febe-42aa-bb0f-477318a58d50.png)


### Here are some of the key outcomes of the project:
- The Air-Passengers Time-Series Dataset was quiet small, with just 144 samples.
- It was clear from the visuals that the time-series dataset had an upward trend & some seasonality.
- The same was confirmed with help of visual (rolling mean & std) & statistical (Dicky-Fuller Test) stionarity checks.
- The time-series was subject to Decomposition in order to stationarize the outputs.
- Futher ACF & PACF curves were plotted to extract the values of p & q, as it is required for the ARIMA Model.
- The Forecasting Model was then built with the time-series data, by feeding the optimal p,q,d values.
- Finally, the model was used to forecast the time-series of the air-passengers, into the future.

