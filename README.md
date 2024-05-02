Citin' the sightings of meteorites!

This project uses this Meteorite Landings dataset compiled by NASA (https://data.nasa.gov/widgets/gh4g-9sfh?mobile_redirect=true), the results of a SPARQL query on Wikidata (https://w.wiki/9xFM), and a dataset created from the Library of Congress' Chronicling America: Historic American Newspapers API (https://chroniclingamerica.loc.gov/about/api/).

We converted the NASA and Wikidata sets to GeoJSON, and we used Mapbox in order to plot them as points on a globe. Using JavaScript, these points are clickable with tombstone data about the meteorites.

The Chronicling America dataset was created by querying the API for the word “meteorite” and pulling the newspaper name, location, and date from those results. Using the OpenStreetMap Nominatim API (https://nominatim.org/), these locations were translated into latitude and longitude coordinates and placed into a new CSV. That CSV was converted to geojson, and we plotted that in Mapbox to represent reporting coverage on meteorites across North America. Using JavaScript, these points are clickable with tombstone data about the coverage.

Our visualization is accessible through the index.html file.
