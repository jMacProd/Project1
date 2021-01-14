# Project1

## Data
2018\calendar_dec_2018.csv
    columns = listing_id,    date,    available
    available is true or false for each date for each listing ID
    Date range from 07/12/2018 - 07/12/2019

2018\listings_2018.csv          *saved as calendar_dec_2018_prelimClean.csv
    calendar_last_scraped: 7/12/18
    Records: 22895
    D - I           Listing profiles - Free text - not useful
    J - T           Host profiles - incl superhost
    U - AH      Accommodation location
    AI - AQ     Accommodation characteristics
    AR - AX     Price
    AY - BF     Availability
    BG - BQ     Reviews - including reviews oer month!!!
   
   Columns Removed: requires_license - license - jurisdiction_names - instant_bookable - is_business_travel_ready - cancellation_policy - require_guest_profile_picture  - require_guest_phone_verification - calculated_host_listings_count (duplicate info)
    
    For host id with multiple listings, the listings can include duplicates but with different information ie Lat: -37.8795903 versus -37.88603312 
    
    city    latitude    longitude    room_type    accommodates    bathrooms    bedrooms    beds    price    guests_included
    Elwood    -37.8795903    144.9916545    Entire home/apt    3    1    1    2    $138.00     2
    Elwood    -37.88603312    144.9882295    Entire home/apt    3    1    1    2    $129.00     2
    Elwood    -37.87383759    144.9886066    Entire home/apt    5    1.5    2    3    $199.00     4

2018\listings_summary_dec18.csv
    calendar_last_scraped: 7/12/18
    Records: 22895 - same as calendar_dec_2018_prelimClean.csv 
    Colums: id    name  -  host_id  -  host_name  -  neighbourhood_group  -  neighbourhood  - latitude  -  longitude   - room_type   - price  -  minimum_nights  -  number_of_reviews   - last_review   - reviews_per_month  -  calculated_host_listings_count  -  availability_365


