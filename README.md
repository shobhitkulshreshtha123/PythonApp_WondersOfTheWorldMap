# PythonApp_WondersOfTheWorldMap
This simple python app locates the 8 wonders of the world on a map

This simple app created on Python allows users to locate 8 wonders of the world. It uses Pandas, Numpy, Folium and Geopy libraries.

Datasource is created at the beginning of program where 7 wonders of the world have been updated in the list

We iterate through our wonder list and search for geocode (Latitude and Logitude) using Nominatim available through Geopy library. If the geocodes are found, they are added in lat and long lists. We convert each latitude and longitude into a tuple and add to another variable called lat_lon.

We use Folium to create a map and add markers based on geocodes available in lat_lon. These markers, when hovered over, displays a shoutout of wonder name. When clicked, these markers return the latitude and logitude of location.

This app can be handy and if integrated with a web scraper for real time automatic updates.
