# Time Series Forecasting with ARIMA
This repository contains the code written for a telecommunications company.

## Problem Statement : 
The company has several thousand cell towers across the country. Each cell tower has certain capacity (data that it is able to process). The time it takes to upgrade a tower's capacity is several months. They wanted to know a year in advance, which towers would be nearing their capacity based off of historical data.

## Solution :
I have designed the ARIMA model provided in the code above to process the historical data for each of their cell towers (1->3 years of weekly peak usage), and then generate 52 predictions. Each prediction represents the peak usage that cell tower will need to process on a given week. 

A mock dataset was used in the jupyter notebook shown above to read in historical data for a few cellular sites, apply the ARIMA machine learning model to each individually, then to make 52 weekly predictions (1 year into the future) and output a graphical image which includes the historical data recorded, and the year long prediction in 52 week incriments.

This code also includes the logic for generating a CSV report which outputs each weekly prediction for a given cellular site and the percent of error that is expected with the prediction. 

### Vocabulary
**% Utilization :** (Data Processed By Cellular Tower) / (Maximum Data that Cellular Tower is able to process)

**EX :** If **Tower A** is able to process a maximum of **1000 GB** of data and currently is processing **500 GB** of data, Tower A's **% Utilization** is **(500) / (1000) = 50%**
