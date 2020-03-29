# Identify Customer Segments for customer data
This project has been completed as part of the [Udacity's Machine Learning Nanodegree](https://www.udacity.com/course/intro-to-machine-learning-nanodegree--nd229) requirements.

## Overview
In this project real-life data are used. These are provided from Udacity's Bertelsmann partners AZ Direct and Arvato Financial Solutions.
Two datasets are used:
- Dataset that contains demographic information about the people of Germany.
- A sedond dataset with that same information for customers of a mail-order sales company in Germany.

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
  
## Requirements
- Python
- Libaries: Sklearn, Pandas, NumPy, MatPlotlib, Seaborn, json, time
- Jupyter Notebook

## Results
The principal component anlysis (PCA) shows that 25 principal components (out of more than 60) explain about 83% of the variability of the dataset.
The most important features of the general population for the first 3 principal components have been identified and discussed.
Clustering has been applied to the general population and the customer data. 8 clusters have been selected to obtain the cluster predictions. Results of the clustering are used to identify the target audience of the company.

***Sreenshots from the analysis:***

*Exploring the ratio of variance explained by each principal component as well as the cumulative variance explained:*

<p align="center">
  <img src= "https://github.com/gepallas/Machine_Learning_3_Customer_Segmentation/blob/master/img1_explained_variance_per_component.png?raw=true" />
</p>


*Investigating the change in within-cluster distance across number of clusters:*

<p align="center">
  <img src= "https://github.com/gepallas/Machine_Learning_3_Customer_Segmentation/blob/master/img2_avg_distance_to_cluster_center.png?raw=true" />
</p>


*Comparing the proportion of data in each cluster for the customer data to the proportion of data in each cluster for the general population:*

<p align="center">
  <img src= "https://github.com/gepallas/Machine_Learning_3_Customer_Segmentation/blob/master/img3_data_distr_per_cluster.png?raw=true" />
</p>
