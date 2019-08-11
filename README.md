# An end-to-end data science project using historical weather data from Singapore

## By Chua Chin Hon
### Github Repo Title: weather_singapore_cch

## SUMMARY
For data science students in Singapore, it is hard to find detailed, yet publicly available local datasets for lessons or personal projects. I came across a [multi-decade collection of weather data](http://www.weather.gov.sg/climate-historical-daily/) on the Singapore Met Service's website by chance, and decided to assemble it for future use, or in case the data is taken offline. 

I'm also using the dataset for a series of self-assigned data science projects, starting with visualisation. I intend to include time series and machine learning forecasts in future updates to this project.  

## TABLE OF CONTENT
There are 3 sections so far. The original CSV files containing the daily and monthly weather data are in the raw folder. Those who want to assemble their own datasets should head there first.

The data folder contains lightly processed CSV files for weather data from 1983 to June 2019. Those who want to quickly test out a model can start with those files.

The notebook folder has two files currently, one on data pre-processing and the other on visualisation. I intend to add more going ahead.

## I. DATA COLLECTION-PREPROCESSING
What you'll find in the [raw folder](https://github.com/chuachinhon/weather_singapore_cch/tree/master/raw):

* 438 CSV files containing daily weather data for Singapore from 1983 - 2019 (June)

* A "monthly_data" sub-folder containing monthly average data for rainfall, maximum and mean temperatures.

What you'll find in the [data folder](https://github.com/chuachinhon/weather_singapore_cch/tree/master/data):
* 4 CSV files processed in the notebook [1.0_data_cleaning_cch](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/1.0_data_cleaning_cch.ipynb) 


## II. EDA & DATA VISUALISATION
The lack of seasonal variations lull many into thinking that Singapore's weather is predictable and unchanging. Nothing is further from the truth, with climate change making the city state's weather even more unpredictable.

In notebook [2.0_visualisation_cch](2.0_visualisation_cch.ipynb), I'll attempt to illustrate the changing weather patterns in Singapore using classic as well as new visualisation libraries/techniques like Plotly Express.

# CONTACT
### Twitter: @chinhon
### LinkedIn: www.linkedin.com/in/chuachinhon