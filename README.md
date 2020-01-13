# An end-to-end data science project using historical weather data from Singapore

## By Chua Chin Hon
### Github Repo Title: weather_singapore_cch

## SUMMARY
For data science students in Singapore, it is hard to find detailed, yet publicly available local datasets for lessons or personal projects. I came across a [multi-decade collection of weather data](http://www.weather.gov.sg/climate-historical-daily/) on the Singapore Met Service's website by chance, and decided to assemble it for future use, or in case the data is taken offline. 

I'm also using the dataset for a series of self-assigned data science projects, starting with visualisation. I will include time series and machine learning forecasts in future updates to this project.  

## TABLE OF CONTENT
There are 5 sections so far. The CSV files containing the daily and monthly weather data are in the raw folder. Those who want to assemble their own datasets should head there first.

## I. DATA COLLECTION-PREPROCESSING
What you'll find in the [raw folder](https://github.com/chuachinhon/weather_singapore_cch/tree/master/raw):

* 444 CSV files containing daily weather data for Singapore from 1983 - 2019 (Dec)

* A "monthly_data" sub-folder containing monthly average data for rainfall, maximum and mean temperatures.

What you'll find in the [data folder](https://github.com/chuachinhon/weather_singapore_cch/tree/master/data):
* 4 CSV files processed in the notebook [1.0_data_cleaning_cch](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/1.0_data_cleaning_cch.ipynb) 

* 2 CSV files related to outlier detection, as processed in the notebook [3.0_outlier_detection_cch.ipynb](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/3.0_outlier_detection_cch.ipynb)

* 1 CSV file related to the Q3 2019 scorcher in Singapore

* 1 CSV file related to the notebooks for machine learning and deep learning, as processed in [notebook5.0](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/5.0_data_prep_cch.ipynb) and 1 validation dataset. 


## II. EDA & DATA VISUALISATION
The lack of seasonal variations lull many into thinking that Singapore's weather is predictable and unchanging. Nothing is further from the truth, with climate change making the city state's weather even more unpredictable.

In notebook [2.0_visualisation_cch](2.0_visualisation_cch.ipynb), I'll attempt to illustrate the changing weather patterns in Singapore using classic as well as new visualisation libraries/techniques like Plotly Express.

Medium post: [Visualising Singapore’s Changing Weather Patterns: 1983–2019](https://towardsdatascience.com/visualising-singapores-changing-weather-patterns-1983-2019-a78605fadbdf)

## III. OUTLIER DETECTION

Data visualisation provide an easy way to spot outliers. But when you have 36 years of weather data, it won't be enough or efficient to rely solely on charts to accurately pick out the outliers.

In the [third section of this project](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/3.0_outlier_detection_cch.ipynb), I'll use Scikit-learn's Isolation Forest model as well as the PyOD library (Python Outlier Detection) to try to pinpoint anomalies in the dataset. This is also important pre-work for Part IV of the project - time series forecasting, where removal of the outliers would be key to more accurate predictions.

Medium post: [Detecting Abnormal Weather Patterns With Data Science Tools](https://medium.com/p/detecting-abnormal-weather-patterns-with-data-science-tools-5fae48586469?source=email-b3d8090c0aee--writer.postDistributed&sk=7871a6d09463983910eff9cc9a684b6b)


## IV. Scorcher: Q3 2019 temperature records

This [fourth notebook](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/4.0_scorcher2019_cch.ipynb) is a short follow-up of sorts to Part II, looking at how temperatures during the three months between July and September 2019 were among the warmest Singapore had experienced over the last 36 years, as global temperature records tumbled around the world.

Medium post: [SCORCHER: As Global Records Tumbled, S’pore Baked Under One Of The Warmest Q3 Ever](https://medium.com/@chinhonchua/scorcher-as-global-records-tumbled-spore-baked-under-one-of-the-warmest-q3-ever-436837cb5b0?sk=30523f141ca9934722165e51251592c6)


## V. Weather Predictions: ‘Classic’ Machine Learning Models Vs Keras

You are ready to dip your toes into deep learning but not sure where to start. One way is to build on what you've been doing in Scikit-learn, and apply useful features like pipelines and grid search via the Keras wrappers.

This fifth series of notebooks starts with a [simple example](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/5.1_ml_LR_XGB_cch.ipynb) on pipeline construction and grid search for a binary classification problem, using the Logistic Regression and XGBoost Classifier.

In [notebook 5.2](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/5.2_dl_keras_gridsearch_cch.ipynb), I tackled the same problem using the Keras Classifier, which introduces the concept of defining and building a Keras sequential model. 

In [notebook 5.3](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/5.3_dl_keras_tuner_cch.ipynb), I experimented with the relatively new Keras Tuner as an alternative to the Scikit-learn/grid search approach.

Data preparation for this section of the project are in [notebook 5.1](https://github.com/chuachinhon/weather_singapore_cch/blob/master/notebooks/5.0_data_prep_cch.ipynb). The validation dataset is [here](https://github.com/chuachinhon/weather_singapore_cch/blob/master/data/weather_dec2019.csv).

Medium Post: https://bit.ly/2QJdrpD

# CONTACT
### Twitter: @chinhon
### LinkedIn: www.linkedin.com/in/chuachinhon