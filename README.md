# Overview
The purpose of this project is to extract information from [Mars News](https://redplanetscience.com/) website and [Mars Temperature Data](https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html) website via both automated browsing with Splinter and HTML parsing with Beautiful Soup. Information stored in HTML tables and recurring elements such as multiple news articles on a webpage are extracted. The requirement is to scrape, organize, analyze, and visualize the data. 

The deliverables of this project are:
- Scrape titles and preview text from Mars news articles and export the data into a JSON file
- Scrape and analyze Mars weather data, which exists in a table

This document explains the steps taken to produce the deliverables. They are:
- Collecting data
- Organizing and storing data
- Analyzing data
- Visually communicating the insights

# Results

## Scrape Mars News website and store the scraping results in Python data structures 

![image](https://user-images.githubusercontent.com/31812730/200179740-b577de65-c0ad-4d10-aa7e-55b79c499e3c.png)

Scrapped data is stored in beloe JSON and CSV files
- news_list.json
- News_list.csv

## Scrape and Analyze Mars Weather Data

### Manually scrape the data by using Splinter and Beautiful Soup and assemble the scraped data into a Pandas DataFrame

![image](https://user-images.githubusercontent.com/31812730/200180634-814ce211-2806-4490-82fe-42d2df88a42a.png)

### Examine the data types of all the DataFrame columns

![image](https://user-images.githubusercontent.com/31812730/200180742-a0afa493-bb63-4669-995e-17a91b1da828.png)

### Cast the data to the appropriate datetime, int, or float data types

![image](https://user-images.githubusercontent.com/31812730/200180831-47b6dc40-1b4d-432c-8dea-c7cc3a08e6bb.png)

Scraped data is stored in below CSV file:
- mars_temp_data.csv

## Summary

The analysis provides the following insights:

- Mars has 12 months
- There are 1867 Martian days worth of data exist in the Mars Weather dataset
- Month 2 & 3 are the coldest months at -83 Celsius and month 7 is the warmest month at -68 Celsius in Mars at the location of Curiosity

![image](https://user-images.githubusercontent.com/31812730/200181608-948f3a4d-4fb6-45fa-8a79-6b38e293abad.png)

- Month 6 has the lowest atmospheric pressure at 745.054422 and moth 9 has the highest atomspheric pressure at 913.30597

![image](https://user-images.githubusercontent.com/31812730/200182025-7ef0c65e-391a-4073-9985-47cca159d992.png)

- There are 686 terrestrial days exist in a Martian year (calculated using solar longitude data in the scraped dataset)
- Below chart supports that calculation as there are clearly 3 temperature cycles in 2,000 days 

![image](https://user-images.githubusercontent.com/31812730/200182262-a9b556e7-f6a6-49c3-a918-eba7994afac6.png)





