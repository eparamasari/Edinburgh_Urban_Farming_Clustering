# Researching the Best Place to Start Urban Farming Spots in Edinburgh

## Leveraging Foursquare API and clustering

Edinburgh, the capital of Scotland, is a relatively small but vibrant city with various types of restaurant, often bustling with international tourists.

This project researches the best location for urban farming in the city.
The United Kingdom has been going through [the worst economic shrink](https://www.forbes.com/sites/roberthart/2021/02/12/uk-hit-by-worst-economic-contraction-on-record-amid-covid-19-pandemic/) due to the [lockdown restrictions](https://www.cnbc.com/2021/02/22/uk-lockdown-details-and-dates-of-how-it-could-be-lifted.html) caused by the Covid-19 pandemic. [Food prices have gone up](https://www.theguardian.com/business/2021/feb/17/uk-inflation-rises-as-price-of-food-and-furniture-increases) and many people need more affordable food with constant supply. Some communities are initiating urban farming in the city of Edinburgh, which is also experiencing such economic condition. This project aims to find the best location for these urban farming spots.

This research uses Foursquare API to analyze the best area in Edinburgh to start an urban farming spot based on surrounding venues. Clustering is also used to divide Edinburgh into different clusters, infer the characteristics of each cluster, then decide on which cluster/area is the best for the location of urban farming spots, based on the venues found in that area.

## The Data

The data used was downloaded from [doogal](https://www.doogal.co.uk/PostcodeDownloads.php), and the specific link to download the Edinburgh post codes csv file is [here](https://www.doogal.co.uk/UKPostcodesCSV.ashx?Search=EH). The data has been previously downloaded and is now accessible at [my repo](https://github.com/eparamasari/Coursera_Capstone/blob/main/data/EH-postcodes.csv).

It has 50 columns, but not all columns are necessary for the research, so initial data cleaning will be performed prior to analysis. The columns post code, latitude and longitude coordinates, ward, rural/urban, output area will be useful as identification, and the latitude and longitude coordinates will especially be used in the http requests to Foursquare API. The rural/urban will also be used to analyze whether it will be a good place to open a new restaurant, since we would want an area with a lot of visitor activities.
