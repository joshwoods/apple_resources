

- MapKit JS
- mapkit
-  Displaying Indoor Maps with MapKit JS 

Sample Code

# Displaying Indoor Maps with MapKit JS

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest in your browser.

Download

## Overview

This sample uses the importGeoJSON method from MapKit JS to import data in Indoor Mapping Data Format (IMDF), and render an indoor map in your browser. The sample app demonstrates decoding, rendering, and styling of a small subset of the IMDF feature types and properties.

Use these examples to create your own indoor map with a style that is consistent with your app’s design. You can handle feature categories specific to your venue, and configure the map style using your own colors, icons, and level picker.

Note

This sample code project is associated with WWDC 2019 session 241: Adding Indoor Maps to your App and Website.

### Configure Your Sample Code Project

To run this sample code:

- Run a web server to serve the assets in a directory for the project.

- Host the directory `Dinoseum`, and its content, at the root of your web server.

- Generate a MapKit JS token and copy it into the `jwtoken` file within the `Dinoseum` directory. For more information, see Creating and using tokens with Maps Server API.

## See Also

### Geographical features

importGeoJSON

Converts imported GeoJSON data to MapKit JS items.

GeoJSONDelegate

A delegate object that controls a GeoJSON import to override default behavior and provide custom style.

ItemCollection

A tree structure containing annotations, overlays, and nested item collection objects.

