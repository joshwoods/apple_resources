

- MapKit JS
-  mapkit.Style 

Class

# mapkit.Style

A set of observable attributes for overlays, including the color and opacity of strokes and fills, and line styles.

MapKit JS 5.0+

``` source
interface mapkit.Style
```

## Overview

You can assign a `mapkit.Style` object to an overlay to customize its appearance, such as changing the opacity of the fill or the thickness of the stroke. Style properties are observable, so MapKit JS automatically reflects any change to a style property on the corresponding overlays.

## Topics

### Creating a style

mapkit.Style

Creates and initializes a style object.

StyleConstructorOptions

Initial values of options for applying style to overlays.

### Styling fills

fillColor

The fill color of a shape.

fillOpacity

The opacity of the fill color.

fillRule

A rule for determining whether a point is inside or outside a polygon.

### Styling lines

lineCap

The style to use when drawing line endings.

lineDash

An array of line and gap lengths for creating a dashed line.

lineDashOffset

The number of CSS pixels to use as an offset when drawing a line’s dash pattern.

lineJoin

The corner style to apply when joining line segments.

lineWidth

The width of a line’s stroke, in CSS pixels.

lineGradient

The gradient to apply along the line.

mapkit.LineGradient

A line that displays with a gradient along the length of the line.

### Styling strokes

strokeColor

The stroke color of a line.

strokeOpacity

The opacity of the stroke color.

strokeStart

The unit distance along the line where a stroke begins.

strokeEnd

The unit distance along the line where a stroke ends.

## See Also

### Overlays

Adding interactivity to overlays

Configure and respond to overlays to make them interactive.

mapkit.Overlay

An abstract base object that defines the methods and attributes for map overlays.

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

