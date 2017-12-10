![alt text](https://github.com/didiooi/CivicAirBnB/blob/master/gallery.jpg "CivicAirBnB Logo")

We are interested in how turning home sharing data and GIS into meaningful visualization can elucidate and address various civic issues, including gentrification, affordable housing, small business development, and youth employment.This project was done in conjunction with Houston Hackathon 2017.

# What it does
CivicAirbnb uses the power of data visualization to make neighborhood-specific home sharing data useful to city planners, policymakers, and community organizers in addressing a wide range of civic issues, including gentrification, affordable housing, small business development, and youth employment.

# Accomplishment
- This is the first time Houston-specific Airbnb data has been scraped and analysed.
- Being able to visualize home-sharing data
- Able to visualize Hotel Occupancy Tax income to the city from home sharing

# How we built it
Data Collection:
The web scraping code was written in python 3. It scraped data from the Airbnb and stored the results in a PostgreSQL database.

## Boundary Mapping:
Shapefiles for designated Super Neighborhoods were obtained from the City of Houston GIS Open data website (http://cohgis-mycity.opendata.arcgis.com/datasets/super-neighborhoods).

## Terminology
Super Neighborhood: A super neighborhood is a geographically designated area where residents, civic organizations, institutions and businesses work together to identify, plan, and set priorities to address the needs and concerns of their community. The boundaries of each super neighborhood rely on major physical features (bayous, freeways, etc.) to group together contiguous communities that share common physical characteristics, identity or infrastructure. The super neighborhood elects a council comprised of area residents and stakeholders that serves as a forum to discuss issues and identify and implement priority projects for the area.

## Data Visualizations:
Data analytics and visualization were done in Tibco Spotfire 7.0 and Tableau which is free for NGO use. GIS mapping was done in QGIS an open-source GIS software and base map is obtained from Google Earth Pro using CRS WGS84.

## Visualizations Created:
1. Gaussian distribution of home-sharing by neighborhood
2. Gaussian distribution of home-sharing prices per night by neighborhood.
3. Tree map of neighborhood home-sharing listings by neighborhood
4. Tree map of reviews per listing by neighborhood
5. GIS chart to show distribution of home-sharing listing with markers colored by average price per night.
6. Distribution of Hotel Occupancy Tax (HOT)

## Challenges We Ran Into:
- Difficulty scraping of data from Airbnb, had to use multiple IP addresses
- Proxies were used to estimate hosts' income and number of nights booked (there is about 8% error)

# What's Next For CivicAirBnB
1. Compare geospatial data with youth unemployment addresses to link Hire Houston Youth participants to home sharing hosts to assist in cleaning, preparation of homes/rooms (part time summer job).
2. HOT tax estimates based on average occupancy and daily rate
Estimated overlap between AirBNB guests and hotel guests (to determine what % of AirBNB guests would not have stayed in a hotel, and therefore are a net gain to the HOT)
3. Estimated price premium based on average daily rates — comparison between hotels and Airbnbs in select neighborhoods. i.e. who is paying more for roughly the same product?
4. Fill in gaps of West U and Bellaire with new data scraping
5. Understand distribution of average daily rate (ADR) based on census tract, predominant race and median household income
6. Understand ratio of ADR by census tract to median household income
7. Look at ADR based on proximity to public transit
8. Compare stock, quantity and ADR by council district, congressional distric, school board district et cetera.

# What We Learned
1. Airbnb listings are very underrepresented in neighborhoods that are going through gentrification  
2. Majority of listings are within the $10-20 per night (which utilizes garage or sofa) which shows the popularity of low price  

# Links
[Google Doc Presentation](goo.gl/YBB4Nm)  
[DevPost](https://devpost.com/software/civicairbnb)  
[Video Link, ff to 54:00](https://youtu.be/GWyWWhNRD6c)  
