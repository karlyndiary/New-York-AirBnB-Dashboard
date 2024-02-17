# Seattle Airbnb Analysis (2022)

This is a 2022 analysis of the Airbnb dataset in Seattle. The analysis aims to understand the current state of the Airbnb market in the city and identify trends and patterns in the year 2022. The analysis focuses on factors that impact Airbnb prices, such as the average price by year, average price for the top 5 and bottom 5 neighbourhoods, host residing in the same area as the Airbnb neighbourhood, availability in each neighbourhood on Dec 25th and more.

## Background Information

Airbnb is an immensely popular global platform that was established in 2008. It offers individuals the opportunity to rent out their properties, including homes and apartments, to travellers who need accommodation. Hosts have the freedom to list their space, set prices and availability, and directly communicate with potential guests. Travelers, on the other hand, can search for suitable accommodations based on their preferences, location, and budget. This innovative service provides a more affordable and convenient alternative to conventional hotels, while also enabling travelers to experience local communities and neighbourhoods uniquely. With millions of listings in over 220 countries and regions, Airbnb has revolutionized the travel industry.

## Dataset Source
[http://insideairbnb.com/get-the-data/](http://insideairbnb.com/get-the-data/)

## Tool used
* Microsoft Power BI: Pre-Processing and Data Visualization

### Steps to import data as a folder
1. Get data -> More -> All -> Folder -> Connect -> Path leading to the folder dataset -> Click ok
2. Click on transform data -> Duplicate the file -> Click on Binary to expand the dataset (Repeat the set for the no of datasets)

### Pre-Processing
- The neighbourhood dataset has the headers in the data fields -> select row 1 -> Transform tab -> Click Use first row as headers
- Remove the neighbourhood_group and license columns as it is empty
- Adding new columns: Extracting information from the name column
    - bedrooms, beds, baths, reviews: Duplicate the column ->
        - Transform tab -> Extract -> Text between delimiters -> Rename the column [or]
        - Transform tab -> Split column -> By Delimiter -> Rename the columns
    - reviews - Repeat the same for the star as well

## Dashboard

[https://public.tableau.com/app/profile/karen.judelyn.fernandes](https://public.tableau.com/app/profile/karen.judelyn.fernandes/viz/AirbnbDashboard_16806756909830/Dashboard)

![Airbnb Dashboard](https://user-images.githubusercontent.com/116041695/232975222-c933dd6e-7bce-4c30-b788-647b0f9ac9ab.png)

## Insights

- The Average Price of the Top 5 and Bottom 5 neighbourhoods. 

The bar chart presents a comparison of the average prices in the top 5 and bottom 5 neighborhoods. It reveals that there is a significant price difference of approximately $200 among the top 5 neighborhoods, whereas the bottom 5 neighborhoods show only slight variations in their average prices.

- The Comparison between the Neighbourhood's Average Price and the Total no of Baths & Beds

The bar chart presents data on the number of beds and baths in different neighborhoods and reveals an interesting trend. Surprisingly, it shows that listings with 1 bath and 1 bed are priced slightly higher than those with 1.5 baths and 1 bed, whereas listings with 2 beds show a gradual increase in price with an increase in the number of baths. This indicates that the relationship between beds, baths, and pricing may not follow a linear pattern, as listings with different bed and bath combinations may have varying pricing structures across neighborhoods.

- Total number of Room Types

The bar chart provides a visual representation of the distribution of room types available on Airbnb in Seattle. The data shows that the majority of room types are entire homes/apartments, accounting for 86.01% of the listings. Private rooms make up 13.85% of the listings, while shared rooms constitute a minimal portion at 0.14%. This suggests that Airbnb in Seattle generates the most revenue from entire home/apartment listings, which are the most prevalent room type.

- Availability in each neighbourhood on Dec 25th

The horizontal chart displays the availability of Airbnb listings in various neighborhoods on December 25th. The University District stands out as the neighborhood with the highest number of available listings, totaling 69 for Christmas bookings. On the other hand, neighborhoods like Roxhill and Harbour Island have considerably fewer Airbnb listings available for booking on that date, indicating limited availability in these areas.

- Average Price for 2022

The highest average prices are observed in July, which corresponds to the summer season in Seattle. This could be attributed to increased demand for bookings during the peak summer vacation period. On the other hand, the lowest average prices are recorded in January, which is the coldest month in Seattle. Interestingly, this trend is consistent for both entire homes/apartments and private rooms. However, when it comes to shared rooms, there is no variation in the average price throughout the year.

- Host residing in the same area as the Airbnb neighbourhood

The Belltown area has the highest number of Airbnb hosts who reside in the neighbourhood, with a total of 22 hosts. In contrast, the East Queen Anne area has a relatively lower number of hosts, with 10 hosts residing in the neighbourhood.

- Top 10 Hosts with the most reviews

Blueground has received the highest number of reviews among all hosts, totalling 5460 reviews. On the other hand, Jian has received the least number of reviews with a total of 270 reviews.
