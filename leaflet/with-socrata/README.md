# Leaflet Maps with Socrata API Open Data

*By [Jack Dougherty](../../introduction/who.md), last updated December 21, 2016*

**TO DO** insert sample map iframe

## Why pair Leaflet maps with Socrata data?

Leaflet, a friendly and flexible open-source code library for creating interactive web maps, plays nicely with Socrata, an open data platform used by several government agencies and organizations. Benefits of pairing Leaflet and Socrata:

- Although the Socrata data platform includes built-in visualization tools for anyone to create charts and maps, Leaflet gives you more control over your map design. Furthermore, Leaflet allows you to create maps that bring together data from both Socrata and non-Socrata sources.
- Socrata datasets include an API (application program interface) endpoint, in the form of a web address. This endpoint enables other computers to easily access the most recent data online, instead of a static version that was manually downloaded.
- Newer Socrata datasets that include locations (such as latitude and longitude coordinates) also provide endpoints in GeoJSON format. Since Leaflet maps easily process GeoJSON data, only a few lines of code are required.

- However, Socrata GeoJSON endpoints do not currently support "real-time" data, such as up-to-the-minute locations of public transportation, etc. In these cases, you may need to access data through a provider other than Socrata, most likely in a different format, which may require more coding skills.

## About Socrata API endpoints

**TODO** clean up my rough notes and add visuals

Go to any Socrata open data platform, find a dataset, and click the API tab

Copy the API endpoint. The default version ends in .json

If you're new to APIs, test the endpoint by pasting it into your browser (Chrome works best at this), and you will see its data stream in JSON format.

Test if this Socrata endpoint supports GeoJSON format by changing the suffix in your browser from ```.json``` to ```.geojson```. GeoJSON format works best with Leaflet because the coding is simpler.

If your endpoint supports GeoJSON format, your browser will display a data stream similar to the one below:

add sample GeoJSON stream

Or if you receive the following error, you probably are viewing an older Socrata endpoint that does not support GeoJSON format, but only JSON format:

```GeoJSON/SoQLPack MimeType is only supported for new backend views```

If your Socrata endpoint only supports JSON format, but includes data columns with latitude and longitude, see other Leaflet examples further below.

## Register for Socrata App Token
- Socrata requires developers to register for a free app token at https://dev.socrata.com/register

## Demonstration Maps

### GeoJSON endpoint with default markers and pop-up info window
- map https://jackdougherty.github.io/leaflet-socrata/index.html
- code https://github.com/jackdoughety/leaflet-socrata/index.html
- data https://data.hartford.gov/Public-Health/Current-Class-1-Class-4-Food-Establishments/xkvv-76v8
- note: location data appears as latitude and longitude coordinates in the ```geom``` column

- steps to create your own   (MORE TODO HERE)

  - select API button, copy endpoint, and change suffix from .json to .geojson

  - copy this Leaflet map template, which includes this key section of code:

  - paste and explain the code

### GeoJSON endpoint with simple data filter, circle marker styling and pop-up info
- map https://jackdougherty.github.io/leaflet-socrata/index-geojson-filter-circle.html
- code https://github.com/jackdoughety/leaflet-socrata/
- data https://data.ct.gov/Environment-and-Natural-Resources/Agricultural-Commoditites-Grown-By-Farmer/y6p2-px98

### Multiple Socrata datasets with Leaflet control layers legend
- map https://jackdougherty.github.io/leaflet-socrata/index-control-layers.html
- code https://github.com/jackdoughety/leaflet-socrata/index-control-layers.html

### Older JSON-only endpoint, with separate columns for latitude, longitude
- map https://jackdougherty.github.io/leaflet-socrata/index-json.html
- code https://github.com/jackdoughety/leaflet-socrata/index-json.html
- data https://opendata.demo.socrata.com/Government/Kentucky-Farmers-Market-Map/3bfj-rqn7

## Learn more
- https://dev.socrata.com/
- https://github.com/chriswhong/simpleSodaLeaflet

## Thanks to
- Chris Metcalf https://github.com/chrismetcalf
- Tyler Klyeklamp https://data.ct.gov/

{% footer %}
{% endfooter %}
