

- MapKit JS
-  StylesOverlayOptions 

Structure

# StylesOverlayOptions

An observable set of style attributes for an overlay.

MapKit JS 5.0+

``` source
dictionary StylesOverlayOptions {
 mapkit.Style style;
};
```

## Overview

The style object is an observable dictionary of style properties. To render an overlay, you must assign a style object to it. The style object specifies attributes, including stroke and fill colors, opacity, and line styles.

Because style properties are observable, MapKit JS automatically reflects changes to a style property on overlays that you associate with that style object.

## Topics

### Overlay style

style

An object literal of style properties.

## See Also

### Creating a circle overlay

mapkit.CircleOverlay

Creates a circle overlay with a center coordinate, radius, and style options.

