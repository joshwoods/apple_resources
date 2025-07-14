

- MapKit JS
-  mapkit.PolylineOverlay 

Class

# mapkit.PolylineOverlay

An overlay of connected line segments that don’t form a closed shape.

MapKit JS 5.0+

``` source
interface mapkit.PolylineOverlay
```

## Mentioned in 

MapKit JS 5

## Overview

A *polyline* is a shape that consists of connected line segments that you define with a set of points. The first and last points don’t connect to each other.

The longitude of all points should be within a 360-degree range. Depending on how you specify the longitude, a line between Tokyo and Los Angeles that you create with a mapkit.PolylineOverlay may take a different route. Specifying a longitude of -118º for Los Angeles and 140º for Tokyo results in a very long line spanning 258º. Specifying a longitude of 242º (that’s, -118 + 360) for Los Angeles and 140º for Tokyo results in a shorter line spanning 98º. MapKit JS may not render the polyline correctly if the range of longitudes is larger than 360º.

All style properties apply to polyline overlays except `fillColor`, `fillOpacity,` and `fillRule`. MapKit JS ignores properties that don’t apply. mapkit.PolylineOverlay doesn’t implement methods of its own. For more information, see the base object, mapkit.Overlay.

The following example shows a polyline object for a map.

```
var points = [ [10, 1], [5, 6], [1, 1] ];
var coords = points.map(function(point) {
    return new mapkit.Coordinate(point[0], point[1]);
});

var style = new mapkit.Style({
    lineWidth: 2,
    lineJoin: "round",
    lineDash: [8, 4],
    strokeColor: "#F0F"
});

var polyline = new mapkit.PolylineOverlay(coords, { style: style });
map.addOverlay(polyline);
```

## Topics

### Creating a polyline overlay

mapkit.PolylineOverlay

Creates a polyline overlay with coordinate points and style options.

StylesOverlayOptions

An observable set of style attributes for an overlay.

### Defining the polyline

points

An array of coordinate points that define the polyline overlay’s shape.

## Relationships

### Inherited By

- mapkit.Overlay

## See Also

### Overlays

Adding interactivity to overlays

Configure and respond to overlays to make them interactive.

mapkit.Overlay

An abstract base object that defines the methods and attributes for map overlays.

mapkit.Style

A set of observable attributes for overlays, including the color and opacity of strokes and fills, and line styles.

mapkit.CircleOverlay

A circular overlay with a configurable radius that centers on a specific geographic coordinate.

mapkit.PolygonOverlay

An overlay consisting of one or more points that forms a closed shape.

OverlayOptions

A dictionary of options that determines an overlay’s data, and indicates whether it’s visible, in an enabled state, and in a selected state.

mapkit.TileOverlay

An overlay that covers an area of the map with bitmapped tiles.

