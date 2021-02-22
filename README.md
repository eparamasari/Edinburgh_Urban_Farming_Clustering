# Researching the Best Place to Open a Restaurant in Edinburgh

## Leveraging Foursquare API and clustering

Edinburgh, the capital of Scotland, is a relatively small but vibrant city with various types of restaurant, often bustling with international tourists.

This project researches the best place to open a new restaurant in the city. Anyone who wants to open a new restaurant in Edinburgh would be able to use the insights from this project.

This research uses Foursquare API to analyze the best area in Edinburgh to open a new restaurant based on surrounding venues. Clustering is also used to divide Edinburgh into different clusters, decide the characteristics of each cluster, then decide on which cluster/area is the best for the location of a new restaurant, based on the venues found in that area.

## The Data

The data used was downloaded from doogal <https://www.doogal.co.uk/PostcodeDownloads.php>, and the specific link to download the Edinburgh post codes csv file is <https://www.doogal.co.uk/UKPostcodesCSV.ashx?Search=EH>. The data has been previously downloaded and is now accessible at <https://github.com/eparamasari/Coursera_Capstone/blob/main/data/EH-postcodes.csv>.

It has 50 columns, but not all columns are necessary for the research, so initial data cleaning will be performed prior to analysis. The columns post code, latitude and longitude coordinates, ward, rural/urban, output area will be useful as identification, and the latitude and longitude coordinates will especially be used in the http requests to Foursquare API. The rural/urban will also be used to analyze whether it will be a good place to open a new restaurant, since we would want an area with a lot of visitor activities.
