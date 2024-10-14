# bigdata_project

## Project Goal
The project focuses on the classification of accidents, allowing users to input information about an accident. The system will then provide information on the severity of the accident.

## Dataset
Download from kaggle, it is a countrywide car accident dataset that covers 49 states of the USA. The accident data were collected from February 2016 to March 2023, using multiple APIs that provide streaming traffic incident (or event) data. The dataset currently contains approximately 7.7 millionaccident records.

The "bigdata_project-main" cotains the zip file of dataset.


## Data Processing
### Feature importance
use a Random Forest classifier to calculate and display the importance of each feature in predicting the 'Severity' label.

### Accidents Distribution Graph
I use fiona, a python library that can read and write geographic data files to create a map that visualizes the geographic distribution of accidents across the United States. It helps in understanding where accidents are concentrated. Show the distribution on the map file, "cb_2018_us_state_500k.shp" in the "bigdata_project-main"

## Clustering
In this context, I choose to use K-means for its simplicity, scalability and flexibility in
handling different feature types to identify high-risk areas and times when accidents are most likely to occur.
I make clustering on features, using both Euclidean and cosine distance measures. The data has been clustered from 5 up to 50 clusters for each measure, with each case involving a maximum of 20 iterations.
To evaluate the K-means algorithm I use the Silhouette score and within-cluster sum of squares distance.

## Classification
 I use various machine learning models to train the system and predict the severity of accidents based on the results from the previous clustering and the accident description. In particular, I am using two different models: a Random Forest Classifier and a Multinomial Logistic Regression.
 
## Web Application
I use Streamlit, a Python framework for creating web application. Users are able to interact with the web page.
