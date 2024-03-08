# New York Airbnb Analysis (2023)

This is a 2023 analysis of the Airbnb dataset in New York City, providing insights into the current state of the market and identifying trends and patterns. The analysis delves into various factors influencing Airbnb prices, including house and room types, the correlation between the number of bedrooms and price, and the availability of accommodations across different neighbourhoods. Additionally, it highlights the top 5 neighbourhoods based on average price and rating, along with an overview of the dataset presented in a concise table format. Furthermore, the analysis explores the top 10 neighbourhoods with the most listings and identifies the top 5 hosts based on ratings. It also investigates the relationship between the number of reviews and ratings, as well as the impact of house type on price. This comprehensive examination offers valuable insights into the dynamics of the New York City Airbnb market in 2023.

## Background Information

Airbnb is an immensely popular global platform that was established in 2008. It offers individuals the opportunity to rent out their properties, including homes and apartments, to travellers who need accommodation. Hosts have the freedom to list their space, set prices and availability, and directly communicate with potential guests. Travelers, on the other hand, can search for suitable accommodations based on their preferences, location, and budget. This innovative service provides a more affordable and convenient alternative to conventional hotels, while also enabling travelers to experience local communities and neighbourhoods uniquely. With millions of listings in over 220 countries and regions, Airbnb has revolutionized the travel industry.

## Dataset Source
[Combined three datasets of New York](http://insideairbnb.com/get-the-data/) 
- Albany, New York, United States
- New York City, New York, United States
- Rochester, New York, United States

## Tool used
* Microsoft Power BI: Pre-Processing and Data Visualization

## Data Model
![Airbnb drawio](https://github.com/karlyndiary/Airbnb-Tableau-Dashboard/assets/116041695/98fba150-dd43-4057-b950-d93ec33ec8ad)

### Steps to import data as a folder
1. Get data -> More -> All -> Folder -> Connect -> Path leading to the folder dataset -> Click ok
2. Click on transform data -> Duplicate the file -> Click on Binary to expand the dataset (Repeat the set for the no of datasets)

### Pre-Processing
- The neighbourhood dataset has the headers in the data fields -> select row 1 -> Transform tab -> Click Use first row as headers
- Remove the license column as it is empty
- Adding new columns: Extracting information from the name column
    - bedrooms, beds, baths, reviews: Duplicate the name column ->
        - Transform tab -> Extract -> Text between delimiters -> Rename the column [or]
        - Transform tab -> Split column -> By Delimiter -> Rename the columns
    - reviews - Repeat the same for the star as well
- Check the data types
- Remove nulls and blanks

## Dashboard
![NYD_page-0001](https://github.com/karlyndiary/New-York-AirBnB-Dashboard/assets/116041695/f02a5410-2598-4489-8de3-a062c72a2a13)
![NYD_page-0002](https://github.com/karlyndiary/New-York-AirBnB-Dashboard/assets/116041695/e8e0eed9-e8c0-483f-9b6b-7d11a96bf9d9)
![NYD_page-0003](https://github.com/karlyndiary/New-York-AirBnB-Dashboard/assets/116041695/18cd8028-2191-46de-a41d-f584c9857408)
![NYD_page-0004](https://github.com/karlyndiary/New-York-AirBnB-Dashboard/assets/116041695/6295d9a8-7852-48f1-9a6b-0d46a1b08fa2)
