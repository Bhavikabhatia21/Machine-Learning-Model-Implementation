# Machine-Learning-Model-Implementation

# Air Pollution Analysis and AQI Prediction using Machine Learning

## Introduction

Air pollution is one of the major environmental problems faced by many countries around the world. Increasing industrial activities, vehicle emissions, and urban development have significantly contributed to the rise in pollution levels. Poor air quality can negatively affect human health and may lead to respiratory diseases, heart problems, and other serious health issues. Because of this, monitoring air quality and understanding pollution patterns has become very important.

The Air Quality Index (AQI) is a measurement used to indicate how clean or polluted the air is in a specific location. It helps people understand whether the air is safe to breathe or if it may cause health problems. Different pollutants such as Carbon Monoxide (CO), Ozone, Nitrogen Dioxide (NO2), and PM2.5 particles contribute to the AQI value.

This project focuses on analyzing global air pollution data and predicting the AQI category using a machine learning model. The project is implemented using the **Python programming language** and executed in **Jupyter Notebook**, which allows easy data analysis, visualization, and machine learning implementation in one environment.

## Project Objective

The main objective of this project is to analyze air pollution data and build a machine learning model that can predict the AQI category based on different pollutant values. The project also aims to visualize pollution data using graphs so that patterns in air quality can be better understood.

The key objectives of this project are:

* To analyze air pollution data from different countries and cities.
* To clean and preprocess the dataset before applying machine learning.
* To visualize pollution data using different types of graphs.
* To build a machine learning model that can predict AQI categories.
* To evaluate the performance of the model using accuracy.

## Technologies Used

This project uses several tools and libraries that are commonly used in data science and machine learning.

* **Python** – The main programming language used to perform data analysis and machine learning tasks.
* **Jupyter Notebook** – Used as the development environment where the Python code is written and executed step by step.
* **Pandas** – A Python library used for data loading, data cleaning, and data manipulation.
* **Matplotlib** – Used for creating visualizations such as histograms, bar charts, and pie charts.
* **Scikit-learn** – A machine learning library used to implement the Decision Tree classification model.

These tools make it easier to handle datasets, visualize information, and build machine learning models.

## Dataset Description

The dataset used in this project contains global air pollution information from different countries and cities. Each row in the dataset represents pollution data for a specific location.

Some important columns present in the dataset include:

* **Country** – The country where the air pollution data was recorded.
* **City** – The city where the air quality measurement was taken.
* **AQI Value** – The overall air quality index value for that location.
* **AQI Category** – The air quality classification such as Good, Moderate, or Unhealthy.
* **CO AQI Value** – The contribution of Carbon Monoxide to the AQI.
* **Ozone AQI Value** – The contribution of Ozone to the AQI.
* **NO2 AQI Value** – The contribution of Nitrogen Dioxide to the AQI.
* **PM2.5 AQI Value** – The contribution of particulate matter (PM2.5) to the AQI.

These pollutant values are used as input features for the machine learning model to predict the AQI category.

## Data Preprocessing

Before building the machine learning model, the dataset needs to be cleaned and prepared. The dataset is first loaded using the Pandas library. The first few rows of the dataset are displayed to understand its structure and the available columns.

Next, missing values are checked using the `isnull()` function. The output shows that some records contain missing values, especially in the Country column. To ensure that the dataset is clean and suitable for analysis, rows containing missing values are removed using the `dropna()` function.

After removing missing data, the dataset becomes ready for visualization and model training.

## Data Visualization

Data visualization is an important step in understanding patterns within the dataset. In this project, three different graphs are created using the Matplotlib library.

The first graph is a **Histogram** that shows the distribution of PM2.5 AQI values. This helps in understanding how particulate pollution values are spread across the dataset.

The second graph is a **Bar Chart** that displays the count of different AQI categories. This graph shows how many locations fall under each air quality category.

The third graph is a **Pie Chart** that represents the percentage distribution of AQI categories. This provides a simple visual representation of the proportion of each air quality level.

These visualizations help in understanding pollution trends and the overall distribution of air quality categories.

## Machine Learning Model

After analyzing the dataset, a machine learning model is built to predict the AQI category. The features used for prediction include:

* CO AQI Value
* Ozone AQI Value
* NO2 AQI Value
* PM2.5 AQI Value

The target variable used for prediction is **AQI Category**.

The dataset is divided into training data and testing data using the `train_test_split()` function. In this project, 80% of the data is used to train the model and 20% is used to test the model's performance.

A **Decision Tree Classifier** is used as the machine learning algorithm because it is simple, easy to understand, and effective for classification problems.

## Model Training and Accuracy

The machine learning model is trained using the training dataset with the help of the `fit()` function. Once the model is trained, predictions are made on the testing dataset using the `predict()` function.

The performance of the model is evaluated using the `accuracy_score()` function. In this project, the model achieved an accuracy of approximately **0.9997**, which indicates that the model performs very well on the dataset.

## Sample Prediction

A sample input is provided to test the model:

CO AQI Value = 50
Ozone AQI Value = 60
NO2 AQI Value = 40
PM2.5 AQI Value = 120

Based on these pollutant values, the model predicts the AQI category as **“Unhealthy for Sensitive Groups.”** This means that the air quality can affect people who are more sensitive to pollution, such as children, elderly individuals, and people with respiratory problems.

## Conclusion

This project demonstrates how Python, Jupyter Notebook, and machine learning techniques can be used to analyze environmental data and predict air quality levels. Data visualization helps in understanding pollution patterns, while the machine learning model provides predictions based on pollutant measurements.

Such systems can help improve environmental monitoring and provide useful insights about air pollution. Predicting AQI categories can help people become more aware of air quality conditions and take necessary precautions to protect their health.
