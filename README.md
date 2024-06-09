# Dynamic Data Map - GitHub Repository

This repository contains code for creating a dynamic data map using Mapbox and fetching data from a Firebase URL. Below are the details of the parameters and URL examples used in the project:

## Parameters

### firebaseurl
- **Description**: Specifies the URL of the Firebase database containing the location data.
- **Type**: String
- **Example**: `firebaseurl=https://your-firebase-url.firebaseio.com/locations.json?auth=your-auth-token`

### category
- **Description**: (Optional) Specifies the category of locations to display on the map.
- **Type**: String
- **Example**: `category=pharmacy`

## URL Examples

### Fetch All Locations
To fetch and display all locations on the map, simply provide the `firebaseurl` parameter without the `category` parameter:

https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM


### Fetch Specific Category
To fetch and display locations of a specific category (e.g., "pharmacy" or "police_station"), provide both the `firebaseurl` and `category` parameters:

https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM&category=pharmacy


## About
This project utilizes Mapbox for map visualization and fetches location data from a Firebase database. It provides a dynamic mapping solution that can be customized to display different categories of locations based on the provided parameters in the URL.
