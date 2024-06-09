
# Dynamic Data Map

This project provides a dynamic map display based on data fetched from a Firebase Realtime Database. It supports two shapes of data and allows specifying a category for display.

## Usage Examples

### Without Category Parameter

Directly fetch and display all spots from a specified URL:

```
https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/parking_spots.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM
```

### With Category Parameter

Fetch and display only the specified category:

```
https://free2510.github.io/map-6/index.html?firebaseurl=https://smart-vilage-default-rtdb.firebaseio.com/locations.json?auth=AIzaSyCSMlIol-7KSVR22X7WS6uceayDyNZM3bM&category=pharmacy
```

## Supported Data Shapes

### Shape 1: Category-based Structure

```json
{
  "pharmacy": [
    {
      "address": "123 St",
      "latitude": 27.272295445302337,
      "longitude": 31.265541752111393,
      "name": "البريد المصري"
    },
    {
      "address": "456 St",
      "latitude": 27.270229574912683,
      "longitude": 31.265317035363662,
      "name": "مصنع شركة سسكو"
    }
  ],
  "police_station": [
    {
      "address": "789 Oak St",
      "latitude": 27.27157798672489,
      "longitude": 31.26747356958013,
      "name": "قسم اول"
    }
  ]
}
```

### Shape 2: Individual Spot Entries with Occupied Status

```json
{
  "spot1": {
    "latitude": 27.2711300032348,
    "longitude": 31.2625760003178,
    "name": "Parking Spot 1",
    "occupied": 1
  },
  "spot10": {
    "latitude": 27.2711046348404,
    "longitude": 31.2626934441832,
    "name": "Parking Spot 10",
    "occupied": 0
  },
  "spot11": {
    "latitude": 27.2710700657154,
    "longitude": 31.2627551349869,
    "name": "Parking Spot 11",
    "occupied": 0
  }
}
```

## Key Features

- **Dynamic Display**: Fetches and displays data dynamically from a Firebase Realtime Database.
- **Category Support**: Supports fetching and displaying data for specific categories.
- **Marker Filtering**: Skips spots with an `occupied` status of `1` to not display them on the map.

Feel free to use and customize this project according to your needs!
