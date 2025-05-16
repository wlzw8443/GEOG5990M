# GEOG5990M


Background & Project Overview
The project investigrates the relationship between pothole severity with socioeconomic deprivation of LSOAs in Leeds. Data for the analysis were obtained from Leeds City Council, Data Mill North, and the UK Data Services, these data were used to determine the differences in potholes count with varying deprivation levels in Leeds.

Data Sources

Data used in this project include:
1) Leeds potholes dataset: Contains reported potholes in Leeds which include coordinates and information regarding report date, completion date, status and other information required by the council. Source: Data Mill North (https://datamillnorth.org/dataset/e7ylx/historic-potholes-data)
2) Index of Multiple Deprivation (IMD): Contains the LSOAs and IMD Deciles of the areas. Source: Leeds Observatory (https://observatory.leeds.gov.uk/deprivation/)
3) LSOA Leeds Boundary: Shapefiles of the Lower Super Output Areas of Leeds. Source: UK Data Service (https://ukdataservice.ac.uk/learning-hub/census/other-information/census-boundary-data/)

Aim of code

The data is firstly cleaned and prepared by:
- Removing missing values and dropping irrelevant columns
- Ensuring CRS is reprojected to EPSG:27700 (British National Grid)
- Convert data to GeoDataFrames

The potholes, IMD and boundary data are:
- spatially joined and merged together to assign potholes to its corresponding LSOA
- Fill LSOAs with missing values with 0

Non-spatial visualisation:
- Boxplot shows the variations and outliers of potholes across deprivation levels
- Linear regression plot displays the strength of the relationship between the variables

Spatial visualisation:
- K-Means Clustering to group LSOAs according to pothole count and deprivation


Futher Information

Install all of the python packages prior to running the codes for the analysis
