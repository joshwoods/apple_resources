

- MapKit JS
-  GeoJSONDelegate 

Class

# GeoJSONDelegate

A delegate object that controls a GeoJSON import to override default behavior and provide custom style.

MapKit JS 5.0+

``` source
interface GeoJSONDelegate
```

## Overview

The delegate object provides hooks into the key moments in the GeoJSON import process. When you pass a delegate object to the importGeoJSON method, you can:

- Modify or replace annotations and overlays before MapKit JS adds them to the ItemCollection object.

- Override the default GeoJSON mapping behavior.

- Provide custom styling by implementing styleForOverlay.

- Receive feedback on the result from importing GeoJSON data.

## Topics

### Overriding items

itemForFeature

Overrides a feature.

itemForFeatureCollection

Overrides a feature collection.

itemForLineString

Overrides a line string.

itemForMultiLineString

Overrides a multiline string.

itemForPoint

Overrides a point.

itemForMultiPoint

Overrides a multipoint object.

itemForPolygon

Overrides a polygon.

itemForMultiPolygon

Overrides a multipolygon.

styleForOverlay

Overrides the style of overlays.

### Handling errors and completion

geoJSONDidComplete

Completes the GeoJSON import.

geoJSONDidError

Indicates when the GeoJSON import fails.

## See Also

### Geographical features

importGeoJSON

Converts imported GeoJSON data to MapKit JS items.

ItemCollection

A tree structure containing annotations, overlays, and nested item collection objects.

Displaying Indoor Maps with MapKit JS

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest in your browser.

