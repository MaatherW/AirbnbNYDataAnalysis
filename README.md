# Airbnb: New York Data Analysis

This analysis is intended for prospective investors evaluating short-term rental property investments in New York City, New York, United States. It employs advanced analytical tools, such as Python and Tableau, to generate insights and offer recommendations through visualizations.

The shared Tableau book link can be accessed [here](https://public.tableau.com/app/profile/ma.ather.waleed/viz/NYAirbnbAnalysis_16930432859280/LocationPopularityBookedListingsDistribution).

## Data Loading And Overview (Python)

The dataset includes four files:

1.  **Listings data** `listings.csv`: Detailed information about each
    listing, including various attributes of the listing (e.g.,
    location, property type, price, availability, number of reviews) and
    the host (e.g., host ID, host listing count).
2.  **Calendar data** `calendar.csv`: Information about the availability and
    price of each listing for different dates.
3.  **Reviews data** `reviews.csv`: Detailed review data for each listing,
    including the date of the review and the comments left by the
    reviewer.

---

![Map based on Longitude and Latitude. Color shows median of Price (Calendar.Csv). The marks are labeled by Counties and % of total booked listings. The data is filtered on Available, which keeps False (booked listings).](https://i.imgur.com/07bXXEm.png)

## Process [(Tableau)](https://public.tableau.com/app/profile/ma.ather.waleed/viz/NYAirbnbAnalysis_16930432859280/LocationPopularityBookedListingsDistribution)


### EDA, Data Cleaning & Filtering

1. Data Collection: view data (calendar + listings+reviews)

    - Select targeted fields, mainly: date (calendar), listing id, location, room type, price (calendar), longitude, latitude, available, Date (reviews), listing id (reviews).

2. Data Cleaning: Missing values and outliers

    In Tableau missing values and outliers can be treated using data source filters:

    - Price (calendar): filter out 0 value
    - Room type: exclude Hotel Rooms

3. Occupancy Rate Field Calculation:

### Visualizations:

-   Location Popularity: Booked Listings Distribution Map
-   Booked Listings VS Median Price Map
-   Location Popularity VS Seasonality
-   Neighborhoods Ranking by Occupancy Rate
-   Neighborhoods Growth since 2017

### Insights and Recommendations

1.  First map: One can easily notice the high density around the center of New York: Manhattan and Brooklyn
2.  Second map shows that the highest % of booked listings are located in Manhattan. And Manhattan has the highest median price. Brooklyn comes in second.
3.  Manhattan ranks first in high booking demand based on the Calendar dataset, uninfluenced by seasonality, Brooklyn comes in second.
4.  Ranking of occupancy rate on neighborhoods levels shows that the top 3 neighborhoods are rather located in Brooklyn.
5.  Top 3 popular locations/neighborhoods: Williamsburg, Bushwick and Bedford-Stuyvesant.
6.  Top 3 growing locations/neighborhoods: Bedford-Stuyvesant, Williamsburg, and Harlem.
