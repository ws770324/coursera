# Scraping

### Github somehow cannot show the folium map, please click [here](https://dataplatform.cloud.ibm.com/analytics/notebooks/v2/33475063-b806-49ce-b0e3-2c7a861078a3/view?access_token=4266a46db055e1095cc8530c10cd14c518db7cb3d49827bc3bf1ecf6377fc8cf) for my whole project 

In this project, I scrape data from wiki, https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M, and explore this data.

First, I use BeautifulSoup to scrape the table. After getting the raw data and cleaning, I merge a data to the origine data to assign latitude and longitude.

For exploring, I use foursquare API to access the information of nearby restaurants and summarize the number of restaurants in each area (postcode). Based on the summary, I assign labels to each area and the range are [0, 10], (10, 25], (25, 50], (50, 75],and (75, 100+]. I visualize these information using folium and found that most of the restaurants are very close to the harbor, and M2J (postcode) has more than 50 restaurants even though it's not very close to the harbor.
