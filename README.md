# Dynamic Map with Firebase Data

This project leverages the Mapbox GL JS library to dynamically display data on a map fetched from a Firebase Realtime Database. By passing URL parameters, you can specify the data source and the category of data to visualize on the map.

## Features

- **Dynamic Data Fetching**: Retrieve data from any Firebase Realtime Database endpoint.
- **Flexible JSON Handling**: Support for both flat and nested JSON data structures.
- **Customizable Map**: Interactive map with customizable markers and popups using Mapbox GL JS.
- **URL Parameter Configuration**: Easily configure the data source and category through URL parameters.

## Usage

### URL Parameters

To customize the data displayed on the map, use the following URL parameters:

- `firebaseurl`: The URL of the Firebase Realtime Database JSON endpoint.
- `category`: (Optional) The specific category within the JSON data to extract and display.

### Example URLs

1. **Pharmacies Data**:
   - Fetches and displays data from the `pharmacy` category.
   - URL:
     ```
     https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations/pharmacy.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM&category=pharmacy
     ```
   - **Description**: This URL fetches information about pharmacies from the specified Firebase endpoint and displays it on the map.

2. **Police Stations Data**:
   - Fetches and displays data from the `police_station` category.
   - URL:
     ```
     https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations/pharmacy.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM&category=police_station
     ```
   - **Description**: This URL fetches information about police stations from the same Firebase endpoint and displays it on the map.

3. **All Categories Data**:
   - Fetches and displays data from all available categories within the JSON.
   - URL:
     ```
     https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations/pharmacy.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM
     ```
   - **Description**: This URL fetches and displays data from all nested categories available in the specified JSON file.

### How to Use

1. Replace `YOUR_FIREBASE_URL` with the actual Firebase Realtime Database JSON endpoint URL.
2. Replace `YOUR_CATEGORY` with the specific category name if you want to filter the data (optional).
3. Open the constructed URL in a web browser.

### Notes

- Ensure the `firebaseurl` parameter is properly URL-encoded if it contains special characters like `&` or `?`.
- If no `category` is specified, all available categories in the JSON will be displayed.

## Dependencies

- [Mapbox GL JS](https://www.mapbox.com/mapbox-gl-js)
- A valid Mapbox access token, which can be obtained from your [Mapbox account](https://account.mapbox.com/).

## Example Map URLs

- **Pharmacies Map**: [View Pharmacies](https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations/pharmacy.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM&category=pharmacy)
- **Police Stations Map**: [View Police Stations](https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations/pharmacy.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM&category=police_station)
- **All Categories Map**: [View All Categories](https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations/pharmacy.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM)

## Project Setup

1. Clone or download the project repository.
2. Open the `index.html` file in your preferred web browser or host it on a web server.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Contributions

Contributions are welcome! Feel free to submit a pull request or open an issue for any improvements or bug fixes.

---

By: [Your Name or Organization]
