# Covid19Precautions-GeospatialDataAnalysis

# Files in the repository:

### Covid19Precautions_GeospatialDataAnalysis_Report.pdf - Detail pdf Report with chart.
### Covid19Precautions_GeospatialDataAnalysis_Presentation.pptx - PowerPoint presentation
### Covid19Precautions_GeospatialDataAnalysi.ipynb - Python code


### 1.Problem Statement:

#### 1.1 Description and Discussion of the Background
The COVID-19 Pandemic, also known as the corona virus pandemic, is an ongoing pandemic of corona virus disease 2019(COVID-19), caused by severe acute respiratory syndrome corona virus 2(SARS-CoV-2). The virus that causes COVID-19 is spreading very easily and sustainably between people. Information from the ongoing COVID-19 pandemic suggest that this virus is spreading more efficiently than influenza, but not as efficiently as measles, which is highly contagious.
The virus is spreading between person-to-person due to close contact, tiny droplets from sneezing, coughing can spread in air and people get infected by touching the contaminated areas and touching their face. As of today, the graph shows the consistent upward arch, while in the other end thing are getting to normal called “new” normal with precautions. But still people find it difficult to get adjusted to new normal, where bringing more risk prone zones for easy contamination.

#### 1.2 Problem
By analyzing the venues of high risky area(where it is highly crowded) and making a legally bonded procedures with extra precautions to handle based on the nature of the venue is an optimal way to control the contamination while we step into the stage of introducing new normal to the people. The idea behind analyzing the venues of Seattle is  due to the constant increase in COVID-19 cases and a big city with large crowd, in future this model can be used in any cities for this purpose as states started slowly announcing to reverse the lock down.

#### 1.3 Interest
Government official to consider extra measures to take precautions and monitor the process to minimize the contamination. General public knowing the high-risk prone areas to undertake extra personnel precautions or to the max avoiding the risk prone areas.


### 2.Data Description
To address this problem and analyze

#### 2.1 Neighborhood data
The data of Seattle Neighborhood is scraped from Wikipedia using BeautifulSoup- python library for web scraping. Wiki table had more column, pulled only district and neighborhood, did not have postal code included- assumed to have unique postal code. Cleaned the data to remove the reference link attached in neighborhood or borough, and to have aligned column.

#### 2.2 Geo-coding
Performing geocoding in python with the help of Geopy and Geopandas libraries to retrieve the geographical coordinates of an address from neighborhood data.

#### 2.3 Venues for clustering
Using the geographical coordinates obtained, the venues are gathered using FourSquare API to perform clustering.

