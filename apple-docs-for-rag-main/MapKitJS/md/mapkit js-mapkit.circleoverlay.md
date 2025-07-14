

- MapKit JS
-  mapkit.CircleOverlay 

Class

# mapkit.CircleOverlay

A circular overlay with a configurable radius that centers on a specific geographic coordinate.

MapKit JS 5.0+

``` source
interface mapkit.CircleOverlay
```

## Overview

The circle overlay provides a built-in object for creating circles. MapKit JS defines mapkit.CircleOverlay by a coordinate and a radius (in meters). All style properties apply to circle overlays except `lineCap`, `lineJoin`, and `fillRule`. MapKit JS ignores properties that don’t apply.

mapkit.CircleOverlay doesn’t implement methods of its own. For more information, see the base object, mapkit.Overlay.

The following example uses circle overlays to show the relative population sizes of three cities in the San Francisco Bay Area:

```
var stats = [
    { name: "San Francisco", coordinate: [37.783333, -122.416667], population: 852469 },
    { name: "Oakland", coordinate: [37.804444, -122.270833], population: 390724 },
    { name: "San Jose", coordinate: [37.333333, -121.9], population: 1000536 },
];

var style = new mapkit.Style({
    lineWidth: 2,         // 2 CSS pixels.
    strokeColor: "#999",
    fillColor: "#FFF"
});

var circles = stats.map(function(stat) {
    var coordinate = new mapkit.Coordinate(stat.coordinate[0], stat.coordinate[1]),
        radius = stat.population / 85, // The radius is in meters.
        circle = new mapkit.CircleOverlay(coordinate, radius);
    circle.data = { population: stat.population };
    circle.style = style;
    return circle;
});

map.addOverlays(circles);
```

## Topics

### Creating a circle overlay

mapkit.CircleOverlay

Creates a circle overlay with a center coordinate, radius, and style options.

StylesOverlayOptions

An observable set of style attributes for an overlay.

### Defining the circle

coordinate

The coordinate of the circle overlay’s center.

radius

The circle overlay’s radius, in meters.

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

mapkit.PolylineOverlay

An overlay of connected line segments that don’t form a closed shape.

mapkit.PolygonOverlay

An overlay consisting of one or more points that forms a closed shape.

OverlayOptions

A dictionary of options that determines an overlay’s data, and indicates whether it’s visible, in an enabled state, and in a selected state.

mapkit.TileOverlay

An overlay that covers an area of the map with bitmapped tiles.

