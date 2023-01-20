# Spotify Song Skip Prediction Challenge

This project is focused on the Spotify Song Skip Prediction Challenge available on AIcrowd.com. The task is to predict whether individual tracks encountered in a listening session will be skipped by a particular user. The project consists of two notebooks that were run on Databricks and make use of Pandas and Pyspark. Pyspark was used in order to make use of big data techniques for my dataset, which is very large.

## Getting Started

To use this project, you will need to have access to a Pyspark environment (I used Databricks) and have the necessary packages (Pandas, Pyspark, etc.) installed.

### Data Sourcing and Ingestion

Data was sourced from the Spotify Song Skip Prediction Challenge at AIcrowd.com. Two files were downloaded in a single tar.gz file and extracted before being ingested into Databricks notebook 1. Spotify supplied two main sets of information. One table has information about user listening sessions. The second table has metadata about the tracks (corresponding to the track_id feature from the session table).

### Exploratory Analysis

Both tables were explored, assessed, and visualized to make inferences and get to know the data. This happened mainly in the first notebook.

### Model

Some feature engineering was carried out, mainly creating new features using data from the previous timestamp. The tables were then joined to create one final dataframe for modeling. A number of different ML techniques were fitted to the data and assessed using MLflow as part of mllib. The best model was chosen using AUC score and results written up.

## Acknowledgements

Data was sourced from the Spotify Song Skip Prediction Challenge at AIcrowd.com.
