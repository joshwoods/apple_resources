

- MapKit JS
-  mapkit.TileOverlay 

Class

# mapkit.TileOverlay

An overlay that covers an area of the map with bitmapped tiles.

MapKit JS 5.0+

``` source
interface mapkit.TileOverlay
```

## Overview

You use tile overlay objects to represent your own tile-based content and to coordinate the display of that content on a map. Your tiles can supplement the underlying map content or replace it completely. You can use a single tile overlay object to represent all of the tiles at one or more zoom levels of the map.

## Topics

### Creating a tile overlay

mapkit.TileOverlay

Creates a tile overlay with a URL template and style options.

TileOverlayConstructorOptions

Attributes for initializing a tile overlay, including minimum and maximum zoom, opacity, and custom data.

### Registering event listeners

addEventListener

Listens for events of the specified type.

removeEventListener

Stops listening for events of the specified type.

### Customizing the tile overlay

urlTemplate

A string, or callback function that returns a string, with a URL that provides the requested tile.

data

A dictionary of custom properties to use with the URL template.

reload

Reloads the tile overlay for the displayed map region with the latest data values.

### Setting overlay appearance

opacity

A number that indicates a tile’s opacity.

maximumZ

The maximum zoom level for a tile overlay.

minimumZ

The minimum zoom level for a tile overlay.

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

OverlayOptions

A dictionary of options that determines an overlay’s data, and indicates whether it’s visible, in an enabled state, and in a selected state.

