

- MapKit
-  MKMultiPolygonRenderer 

Class

# MKMultiPolygonRenderer

The visual representation of multiple polygon overlays.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MKMultiPolygonRenderer
```

## Overview

Use this renderer to provide the style for multiple polygons created using MKMultiPolygon.

## Topics

### Creating a multipolygon renderer

init(multiPolygon: MKMultiPolygon)

Creates and returns a renderer that handles drawing for the specified multipolygon overlay object.

### Accessing the multipolygon object

var multiPolygon: MKMultiPolygon

The multipolygon object that the renderer uses to draw the overlay’s contents.

## Relationships

### Inherits From

- MKOverlayPathRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Custom shape overlays

class MKPolygon

A closed polygon overlay.

class MKPolygonRenderer

The visual representation of a single polygon overlay.

class MKMultiPolygon

A collection of multiple closed polygon overlays.

class MKOverlayPathRenderer

The visual representation of a path-based overlay.

