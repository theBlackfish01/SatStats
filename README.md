# SatStats
SatStats explores the relationship between European land classification data and GDP per capita, aiming to create classification based predictive models for GDP per capita and perform clustering, regression, and classification analysis.

## Dataset: 
The dataset consists of two files:

GDP Data: Obtained From EuroStat. Contains GDP per capita for NUTS3 regions. 

Land Classification Data: Obtained from CORINE datasets, a part of the EU Copernicus Project. Provides land usage statistics with 44 land types for the entirety of Europe, in raster format.

Using QGIS, a vector overlay of the NUTS3 regions was applied and Zonal Histogram generated and outputted to a CSV file. Using the NUTS3 region codes, the files were merged accordingly. Due to the varying sizes of the regions, all classification values were processed into their respective proportions of the region, and then standardized.

## Models:
The main approach to the problem involved implementing a variety of machine learning models tailored to the specific tasks of regression, classification, and clustering. The primary focus was on the classification models.

Classification models - Random Forest Classifier, Support Vector Classifier (SVC), and Logistic Regression

Regression models - Random Forest Regressor, LSTM

Clustering models - K-Means and Hierarchical Clustering

## Results:

LSTM:
![image](data/assets/img.png)

Classification - Random Forest achieved accuracy of 0.767 for data classified into low, medium, and high bins, while the other models were far less effective.

![image](https://github.com/user-attachments/assets/1a3c1d6f-269e-449c-9a20-3cffa088cb95)
![image](https://github.com/user-attachments/assets/209577a1-18d6-40c9-aae9-db614cf23d4c)


Regression - Random Forest achieved R² of 0.55 and Mean Absolute Error (MAE) of 7223.20.

![image](https://github.com/user-attachments/assets/64d969c1-e9c5-4c1e-bed4-ba7c20571772)

KMeans Clustering:

![image](https://github.com/user-attachments/assets/64752ed9-7846-4916-bb4c-9ae249bd0d3a)

