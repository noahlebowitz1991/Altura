# Altura
Uses an autoregressive model to predict future sensible heat in UC Irvine's Hewitt Hall Room 1121. Code made while assisting Altura Associates. Every 15 minutes Altura records data from every room in Hewitt Hall. I used that data to make a time series, then used that time series to predict future results.

There are 5 versions of this code.
v1: I used a linear model to predict sensible heat. Specifically, this just uses a linear AR model on the previous 90 minutes of data. Unfortunately, this model had poor predictive ability.
v2: I replaced the linear model with an XGBRegressor model. I also incorporated daily, weekly, and monthly information.
v3: A streamlined version of v2.
v4: I hypothesized that knowledge of the sensible heat in the neighboring rooms would improve the model. Unfortunately, the model did not improve. I am not ruling out my hypothesis yet, though the model may need to be refined.
v5: I applied the code in v3 to the 14 other rooms in Hewitt Hall Floor 1 where we had enough data.

I cannot legally upload Hewitt Hall data due to an NDA, but I can upload the code I wrote onto GitHub.
