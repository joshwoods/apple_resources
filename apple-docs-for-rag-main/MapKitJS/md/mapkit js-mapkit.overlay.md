

- MapKit JS
-  mapkit.Overlay 

Class

# mapkit.Overlay

An abstract base object that defines the methods and attributes for map overlays.

MapKit JS 5.0+

``` source
interface mapkit.Overlay
```

## Mentioned in 

Handling map events

Adding interactivity to overlays

## Overview

Overlays inherit from an abstract base object, mapkit.Overlay, and share some common properties with mapkit.Annotation that allow you to control the visibility and interaction with the map in the same way. This object is abstract and you can’t instantiate it.

## Topics

### Registering event listeners

addEventListener

Starts listening for the specified type of event.

removeEventListener

Stops listening for the specified type of event.

### Setting overlay options

data

Custom data to associate with the overlay.

visible

A Boolean value that determines whether an overlay is visible.

enabled

A Boolean value that determines whether the overlay responds to user interaction.

selected

A Boolean value that indicates whether the user selects the overlay.

style

Style properties to apply to the overlay.

map

The map you add the overlay to.

## Relationships

### Inherits From

- mapkit.CircleOverlay
- mapkit.PolygonOverlay
- mapkit.PolylineOverlay

## See Also

### Overlays

Adding interactivity to overlays

Configure and respond to overlays to make them interactive.

mapkit.Style

A set of observable attributes for overlays, including the color and opacity of strokes and fills, and line styles.

mapkit.CircleOverlay

A circular overlay with a configurable radius that centers on a specific geographic coordinate.

mapkit.PolylineOverlay

An overlay of connected line segments that don’t form a closed shape.

mapkit.PolygonOverlay

An overlay consisting of one or more points that forms a closed shape.

OverlayOptions

A dictionary of options that determines an overlay’s data, and indicates whether it’s visible, in an enabled state, and in a selected state.

mapkit.TileOverlay

An overlay that covers an area of the map with bitmapped tiles.

