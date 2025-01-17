# SatStats
SatStats explores the relationship between European land classification data and GDP per capita, aiming to create predictive models for GDP per capita and perform clustering, regression, and classification analyses.

## Dataset: 
The dataset consists of two files:

GDP Data: Obtained From EuroStat. Contains GDP per capita for NUTS2 regions. The "geo" column provides the NUTS2 region codes.

Land Classification Data: Obtained from CORINE datasets, a part of the EU Copernicus Project. Provides land usage statistics with 44 land types for the entirety of Europe, in raster format.

Using QGIS, a vector overlay of the NUTS2 regions was created and Zonal Histogram generated and outputted to a CSV file. Using the NUTS2 region codes, the files were merged accordingly. Due to the varying sizes of the regions, all classification values were processed into their respective proportions of the region, and then standardized.
