---
layout: post
title: Taking on The 2023 WiDS Datathon Challenge
date: 2023-2-10
preview: true
---
![_config.yml](/images/WiDS_title2.png)

A few weeks after graduating from BrainStation, I was invited to join a team of fellow alumni to take on a team data competition. We decided on an inspiring Datathon with Women in Data Science(WiDS).  [The 2023 WiDS Datathon](https://www.widsconference.org/datathon.html) has a transcending goal of mitigating the damage of extreme weather events from climate change by improving weather forecasting models.  The first two notebooks that I have contributed to my team’s progress can be found here, [Github](https://github.com/kmack3990/WiDS-2023-Datathon-Challenge).


### Initial Takeaways


This has been a fun challenge to keep some of the community alive that we built during our online bootcamp.  I still get to meet up with some of my comrades to connect and exchange ideas and stories.  


Employing the skills that I have built upon over the last year plus, continues to be rewarding, satisfying, and challenging. The enjoyment I gain from data cleaning and exploration of large data sets grows. This process, that some find tedious, is soothing, fun, and fulfills my natural curiosity!


In this project, I get another crack at working in time series analysis. Although, the data structure of this time series has proved to be much less difficult to manage and model in relation to that of my capstone. I plan to revisit my capstone soon with the knowledge that I gain. 
  
### Project Status
* Data cleaning and processing is complete.
* Two regression machine learning models have been optimized. 
* Data reduction techniques have been employed.
* Our primary submission into the competition has been submitted.
* Feature engineering and further model development need to be implemented. 


In my capstone project, I analyzed power and meteorological metrics measured at the wind farm.  This project has many similarities in that we are analyzing meteorological metrics and there is a time series component. Fortunately, the data is structured so some of the difficulties in analyzing time-series data can be avoided.


The overall goal of the datathon is to create a model to accurately predict the mean of the minimum and maximum daily temperatures 14 days out.  The idea here is that with fourteen days' notice, extreme weather events could be foreshadowed and necessary precautions could be taken to prevent loss of life and property.  


Within the training and test set there are 514 locations.  At each of these locations meteorological data is given.  Furthermore, there are a large variety of forecasting model metrics like NOAA’s CPC Gauge-Based Analysis of Global Daily Precipitation for each location. 


The data sets are large with 244 features containing hundreds of thousands of entries. The data dictionary that seeks to describe our parameters is somewhat abstract.  I have categorized the parameters and aligned their correlations to our target.
After processing the data, I was able to optimize a Random Forest Regressor and a Multi-layer Perceptron.  The Random Forest Regressor scored better on the contest’s error metric of root mean square error.  To set a baseline, I submitted our predictions for the contest’s test_data and scored a RMSE of 1.91 degrees Celsius.  We are on the leaderboard, but we have work to do to improve upon this metric.  


![_config.yml](/images/RFR_results.png)


Over the next couple weeks, we will investigate the implementation of different methods of feature engineering and look to boost the predictive power of other regression models.  I hope to have a future post with dramatic improvement on this RSME soon!
