# meteorite-sight-cites
Citin' the sightings of meteorites!

This project uses this Meteorite Landings dataset compiled by NASA (https://data.nasa.gov/widgets/gh4g-9sfh?mobile_redirect=true) in conjunction with the Library of Congress' Chronicling America: Historic American Newspapers API (https://chroniclingamerica.loc.gov/about/api/). 

Our workflow is detailed below.

1. Initial data cleanup: We removed any rows with missing values from the dataset.
2. Date range filtering: We filtered the dataset to include only meteorites that landed between 1756 and 1963, aligning with the available newspaper data.
3. Location refinement:  We narrowed down the locations to North America based on latitude and longitude coordinates.
4. Enriched location information: Using geolocation data, we extracted additional details such as state and country for each meteorite landing.
