# Identify Customer Segments of the population that form the core customer base for a mail-order sales company in Germany.
This project has been completed as part of the [Udacity's Machine Learning Nanodegree](https://www.udacity.com/course/intro-to-machine-learning-nanodegree--nd229) requirements.

## Overview
In this project real-life data are used. These are provided from Udacity's Bertelsmann partners AZ Direct and Arvato Financial Solutions. Two datasets are used; one that contains demographic information about the people of Germany; and one with that same information for customers of a mail-order sales company in Germany.

I am using k-means clustering to identify segments of the population that form the core customer base for a mail-order sales company. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns.

The project is structured as follows:
- Data Pre-processing
  - Treat missing data
  - Re-encode features
  - Engineer mixed-type features
- Feature Transformation
  - Impute missing values
  - Feature scaling
  - Dimensionality reduction using Principal Component Analysis (PCA)
- Clustering using k-means algorithm (to the general population and to the customer data)
  - Use k-means Score method to select number of clusters
  - Comparing customer data to demographic data
