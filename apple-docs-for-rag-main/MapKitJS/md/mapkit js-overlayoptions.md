

- MapKit JS
-  OverlayOptions 

Structure

# OverlayOptions

A dictionary of options that determines an overlay’s data, and indicates whether it’s visible, in an enabled state, and in a selected state.

MapKit JS 5.0+

``` source
dictionary OverlayOptions {
 Object data;
 boolean visible;
 boolean enabled;
 boolean selected;
};
```

## Overview

Use OverlayOptions to set the initial state of your overlay and provide the data MapKit JS uses to render it.

## Topics

### Overlay options

data

Custom data to associate with the overlay.

enabled

A Boolean value that determines whether the overlay responds to user interaction.

selected

A Boolean value that indicates whether the overlay is in a selected state.

visible

A Boolean value that determines if an overlay is visible.

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

mapkit.PolylineOverlay

An overlay of connected line segments that don’t form a closed shape.

mapkit.PolygonOverlay

An overlay consisting of one or more points that forms a closed shape.

mapkit.TileOverlay

An overlay that covers an area of the map with bitmapped tiles.

