# WebScapping

**1.** The goal of this project is to demonstrate ability to capture unconventional datasets, clean and store them.
**2.** Connect to BigQuery DataSet and querry the data from it. 


### Web Scrapping 
1. For web scrapping I have use the help of libraries **urllib.request**, **BeautifulSoup** and **pandas**
2. I have used all the field in the table which was present in https://en.wikipedia.org/wiki/List_of_United_States_cities_by_population as well as added additional two field which are Mayou name, and city website as they were the field which seems to be have consistent patten of being in infobox of city wikipedia page.
3. I have hard coded a lot of extraction of colums data but have maintained same style of extraction over all rows. 
4. I have used pandas to convert out python dictionary formated data into cvs file which we later manually upload to google cloud bigquerry dataset 

### Executing BigQuery from python 
1. Here we install the google.cloud.bigquery library
2. We keep our API access key in a secured location and reference it to the Client so that we know which bigquery dataset to connect 
3. We no run our query and get the results for the data