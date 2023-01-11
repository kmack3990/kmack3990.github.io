---
layout: post
title: What I Learned About Time Series Data?
date: 2023-1-11
preview: true
---

After 12 intense weeks of long nights and no weekends learning the in’s and out’s of data science at BrainStation, I submitted my capstone project on Wind Power Forecasting. I am calling this my initial report.  As there is still quite a bit more that I want to do with this project.  My preliminary findings can be found here, Github. 


### Picking my Project Topic and Time Series Modeling

![_config.yml](/images/offshore-wind-farm.jpg)

Everyday we are seeing the impacts of climate change from droughts in the Western United States to coral bleaching throughout our international waters.  The consensus is that we need to take drastic action to reduce our carbon footprint and our reliance on fossil fuels.  I wanted to find a project that would develop a tool set in data science that can help to solve this current environmental predicament.  

I sifted through ideas on energy efficiency and different renewable energy projects, and finally landed on wind power forecasting.  Wind power is an energy resource that continues to take on a larger piece of our electricity generation portfolio.  Unfortunately, the wind does not blow all the time.  If electric grid operators can be informed by more accurate wind forecasts, they can make better decisions on when to revert to other power sources such as battery storage.  According to Shouman’s 2022 report on wind forecasting, as little as a 1% error in forecasted wind speeds could result in a loss of $12,000,000 during a wind facilities life cycle (Shouman, 2022).

Any sort of forecasting incorporates data collection over time.  I was aware that time series modeling incorporated an increased level of rigor, but I didn’t really know what this added level of difficulty entailed. 

### What Did I Learn from Forecasting Wind Power?
 
* Exploratory Data Analysis and Data Processing continues to be fun!
* Predicting the future is hard. 
* Jason Brownlee’s “Machine Learning Mastery” Blog is a great resource.
* Time series modeling is a code that I am still working to fully crack.
* I am excited to now have the time to dig deeper into time series modeling with this project and the WiDS Datathon.

In my capstone project, I analyzed power and meteorological metrics measured from four turbines in EDP Renewables Wind Farm 1.  Cleaning the large data set and uncovering the distributions and correlations among the features was time consuming and some might say arduous.  I, on other the hand, continue to find this process soothing and enlightening.  In all my projects, I truly enjoy uncovering problems and solutions within the data, as well as finding intriguing patterns.     

The data signals in this project had no trend, seasonality, or obvious cyclical pattern.  The nature of the data made traditional time series models such as ARIMA models like the SARIMAX have little predictive power.  

![_config.yml](/images/noisy_data.jpg)

I adapted a process from some of Jason Brownlee’s work on time series analysis.  The concept uses a shifting window to read through a time series, frame by frame, to predict a certain number of time steps out from a number of previous time steps.  This allowed me to transform my dataset to establish an independent and dependent variable for machine learning.  

![_config.yml](/images/walk_forward_validation_function.jpg)

Using Brownlee’s shifting window method and a walk forward validation process, I fit a variety of machine learning models.  I received the best results validating Random Forest Regressor Models and vanilla LSTM models.  

My sticking point right now is developing a pipeline and grid search to comprehensively tune these models.  Although I have developed methods to tune one hyperparameter at a time using the walk forward validation techniques, I have yet to fully implement a machine learning pipeline to comprehensively attack the variety of hyperparameters.  Setting up a pipeline and grid search is generally straightforward with machine learning data that has independent variables and dependent variables that are not related through the dimension of time.  I am still developing strategies to incorporate the walk forward validation in time series data to a machine learning pipeline.  

Having graduated from BrainStation, I plan to really come up with some solutions on how to merge walk forward validation and pipelines to strengthen models on this project.  I have also joined a team to continue this challenge in the Women in Data Science (WiDS) 2023 “Datathon Challenge: Adapting to Climate Change by Improving Extreme Weather Forecasts.”  This datathon will further my experience and grow my expertise analyzing time series data.  

I am excited for my next post with solutions to strengthen predictive time series models using walk forward validation and transformed time series data. 


### Resources:

Brownlee, J. (2016, December 6). Time Series forecasting as supervised learning. MachineLearningMastery.com. Retrieved December 11, 2022, from https://machinelearningmastery.com/time-series-forecasting-supervised-learning/ 

Shouman, E. R. M. (2022, May 13). Wind power forecasting models. IntechOpen. Retrieved December 11, 2022, from https://www.intechopen.com/chapters/81755 



