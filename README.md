# leaflet-challenge

This web application uses Leaflet.js and D3.js to visualize earthquake data from the USGS (United States Geological Survey) API. It displays earthquake locations with circles on a map, where the circle size and color represent the magnitude of each earthquake.

Table of Contents
	- Demo
	- Features
	- Installation
	- Usage
	- Credits

### Demo
You can view a live demo of the project here. (Update with your demo link once available)

### Features
	- Display earthquake locations on an interactive map
	- Circle size and color indicate earthquake magnitude
	- Popup with details (place and time) when clicking on a circle
	- Choose between different base map layers (Street Map, Topographic Map, Grayscale Map)

### Installation
1. Clone the repository:
	git clone https://github.com/Neil7777/leaflet-challenge
2. Navigate into the project directory:
	cd leaflet-challenge
3. Install dependencies:

npm install

### Usage
1. Obtain a Mapbox Access Token:
	- Visit Mapbox and create an account.
	- Create a new access token.
2. Replace the placeholder access token in static/js/logic.js with your Mapbox access token:

let grayscale = L.tileLayer('https://{s}.tile.jawg.io/jawg-light/{z}/{x}/{y}{r}.png?access-token={accessToken}', {
    ...
    accessToken: 'YOUR_MAPBOX_ACCESS_TOKEN'
});

3. Run the application:

	npm start
4. Open your browser and go to http://localhost:3000 to view the application.

### Credits
	- Leaflet.js
	- D3.js
	- USGS Earthquake API
	- Base maps:
		- OpenStreetMap
		- Jawg Maps
		- Mundialis Topographic Map
