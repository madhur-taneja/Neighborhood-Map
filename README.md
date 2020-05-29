# Neighbourhood Map

A single page application featuring a map of your neighborhood or a neighborhood you would like to visit with the functionalities including map markers to identify popular locations or places you’d like to visit, highlighted locations, a search function to easily discover these locations, a listview to support simple browsing of all locations and third-party data about those locations

Open and view the Project using the `.zip` file provided or at my [Github Repository](https://github.com/madhur-taneja/Front-End-Projects) having folder `Neighborhood Map`.

The project is also hosted on [GitHub](https://madhur-taneja.github.io/Neighborhood-Map/).

## Table of Contents

- [Getting Started](#getting-started)
	- [Tools Required](#tools-required)
	- [Installation](#installation)
- [Development](#development)
  - [Part 1: Google Maps API and Foursquare API](#part-1-google-maps-api-and-foursquare-api)
  - [Part 2: Include jQuery and Knockout Javascript](#part-2-include-jquery-and-knockout-javascript)
  - [Part 3: Include CSS file, Bootstrap library and Google Fonts](#part-3-include-css-file-bootstrap-library-and-google-fonts)
  - [Part 4: Creating and coding Javascript in app.js and init.js](#part-4-creating-and-coding-javascript-in-appjs-and-initjs)
- [Running the App](#running-the-app)
- [References](#references)

## Getting Started

The aim of this Project is to make a "Map of a Neighborhood" showing famous local Eating Joints with their ratings.

This project was made from scratch and is a part of Udacity's Front-End Web Developer Nanodegree program. The project will be evaluated by a Udacity code reviewer according to the project [rubric](https://review.udacity.com/#!/projects/2711658591/rubric)

### Tools Required

* [Google Maps API](https://developers.google.com/maps/web/) to load map
* [Foursquare API](https://foursquare.com/developers/app/XQ2I0ONGSSVL1DYQYSK2Q0ERIM5ASTRANA5FRG41HTTXVKQB) to fetch data for the eating joints
* [Foursquare API Explorer] to fetch ratings(or other details if required)
* [Knockout Javascript](http://knockoutjs.com/downloads/knockout-3.4.2.js) to bind data
* [jQuery](https://code.jquery.com/jquery-3.2.1.min.js) (Javascript Library) for easier coding of javascript
* [Bootstrap](https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css) to make the page responsive
* [Google Fonts](https://fonts.google.com/specimen/Pacifico?selection.family=Pacifico) to add stylish text
* [Color-Hex](http://www.color-hex.com/) to add hexa-decimal color codes in css
* [HTML Beautifier](http://www.freeformatter.com/html-formatter.html) to Beautify HTML
* [CSS Beautifier](http://www.freeformatter.com/css-beautifier.html) to Beautify CSS
* [JS Beautifier](http://www.freeformatter.com/javascript-beautifier.html) to Beautify JS
* [Online Markdown Editor](http://dillinger.io/) to test `README.md`
* [Google Maps Animation](https://developers.google.com/maps/documentation/javascript/examples/marker-animations) to animate markers

### Installation

No additional installation is required for this project

## Development

### Part 1: Google Maps API and Foursquare API
* Generate a unique key from [Google Maps API](https://developers.google.com/maps/web/) and create `index.html`.
* Set the center and zoom accordingly
* Sign up on `foursquare.com`, create a new app which which provide `CLIENT_ID` and `CLIENT_SECRET` for that app. These unique ID's will be used for fetching data from `foursquare.com` using `AJAX`

### Part 2: Include jQuery and Knockout Javascript
* Use the above mentioned links and append them in `index.html`

### Part 3: Include CSS file, Bootstrap library and Google Fonts
* Create a `style.css` file in `css folder` with all required styling and link it to `index.html`
* Use the above mentioned link for `Bootstrap` and link it in `index.html`
* Use the above mentioned link for `Google Fonts` and link it in `index.html` and `style.css`

### Part 4: Creating and coding functionalities in app.js and init.js
* Create `initMap` and `navToggle` functions in `init.js`

* Now in `app.js`, create an object of eating joints with their name, coordinates and unique Id generated from [foursquare.com]. Create `Viewmodel` with functions to:
  > Create Markers <br>
    Fetch information for Markers from [foursquare.com] using `AJAX` request <br>
    Create Infowindows with relevent information <br>
    Display information fetched from [Foursquare API Explorer] on clicking them <br>
    Style Markers <br>
    Show selected Marker <br>
    Bind data for `Search Bar` using `Knockout Javascript` <br>
    Show and Hide Markers <br>
    Create, toggle and add features to `Drawing Toolbar` <br>

For details now how these functionalities have been implemented, refer the source code. 

**App is completed! Have fun exploring delicious places!**

## Running the App

* Open the project through the `.zip` file provided and extract file
  > Open `index.html` in the browser of your choice.
* Click on the list or the markers on map to see ratings for that particular Eating Joint
* User the search bar to filter out the restaurants in the list as well as in the map 

## References:
* [Udacity's Github Repository](https://github.com/udacity/ud864)
  > This repository was provided in [Lesson 17](https://classroom.udacity.com/nanodegrees/nd001/parts/e87c34bf-a9c0-415f-b007-c2c2d7eead73/modules/4fd8d440-9428-4de7-93c0-4dca17a36700/lessons/8304370457/concepts/83122494440923) <br>
  References for `SHOW AND HIDE FUNCTIONS FOR MARKERS`, `MARKER STYLING`, `DRAWING TOOLBAR` were taken from [here](https://github.com/udacity/ud864/blob/master/Project_Code_7_Drawing.html). <br>
* Knockout Javascript [Docs](http://knockoutjs.com/documentation/event-binding.html)
* Responsive Navbar from [Codepen](https://codepen.io/simoberny/pen/pJZJQY)
* [Example App](https://github.com/udacity/fend-office-hours/tree/master/Javascript%20Design%20Patterns/P5%20Project%20Overview) provided by Udacity 

[foursquare.com]: <https://foursquare.com/explore?mode=url&ne=28.596279%2C77.060477&q=Food&sw=28.585784%2C77.045778)>
[Foursquare API Explorer]: <https://developer.foursquare.com/docs/explore#req=venues/50d6d789498ee282996ddce4>
