Task Overview: You are provided with a public stock price dataset (e.g., daily closing prices). Your goal is to forecast future stock values. Requirements: ● Implement a traditional statistical model (e.g., ARIMA).. ● Implement a machine learning / deep learning model (e.g., LSTM or Prophet).  ● Compare the performance of different approaches. . ● Use rolling window evaluation to measure forecast accuracy 

Short Report: Model Generalization — ARIMA vs Prophet vs 
LSTM 
Objective of the task: My main objective is to forecast stock closing prices using the 
traditional method, ARIMA and also the Prophet and LSTM models. The models are 
evaluated using metrics such as RMSE and MAPE. The comparison between these models 
are demonstrated below. 
Model 
ARIMA 
RMSE 
217.86 
MAPE 
13.57% 
Generalization Capability 
Moderate - captures 
linear trends but weak 
with nonstationary data 
Prophet 
LSTM 
132.67 
33.28 
8.26% 
0.13% 
Which Model Generalization is better and why 
Strong - models trend 
and 
seasonality 
effectively 
Very 
complex 
strong-learns 
temporal 
dependencies 
and 
nonlinear relationships 
The above table shows that among the three implemented model for the task, LSTM 
demonstrates the best generalization performance. While ARIMA depends on linear 
relationships and assumes stationarity. Prophet uses additive components to model trends 
and seasonality. But LSTM directly learns from the temporal patterns and dependencies 
from sequential data. 
The neural network based approach captures nonlinear and long term dependencies more 
effectively and enable it to adapt to volatile stock market data where trends shift dynamically. 
On the other hand, Prophet remains valuable for interpretable forecasting, especially when 
the data is limited. So, 
● ARIMA: Best for simple, stationary time series 
● Prophet: Best for interpretable forecasts with seasonality 
● LSTM: Best for high performance generalization and nonlinear data learning 
Conclusion: ARIMA/Prophet is perfect as strong baselines and data is limited and business 
time series with clear seasonality and trend changes. LSTM is suitable when have more than 
2–3 years of dense daily data, and ready to perform hyperparameter search and 
regularization. Finally, rolling-window evaluation is good to select the final model and to 
estimate real-world performance.
