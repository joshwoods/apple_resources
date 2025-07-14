

- MapKit
-  MKMultiPolygon 

Class

# MKMultiPolygon

A collection of multiple closed polygon overlays.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MKMultiPolygon
```

## Overview

Use a MKMultiPolygon when you have multiple distinct polygon shapes that you intend to render using the same style.

## Topics

### Creating a multipolygon

init([MKPolygon])

Creates a multipolygon object using the provided polygons.

### Accessing polygons

var polygons: [MKPolygon]

An array containing the polygons that make up the multipolygon object.

## Relationships

### Inherits From

- MKShape

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- MKGeoJSONObject
- MKOverlay
- NSObjectProtocol

## See Also

### Custom shape overlays

class MKPolygon

A closed polygon overlay.

class MKPolygonRenderer

The visual representation of a single polygon overlay.

class MKMultiPolygonRenderer

The visual representation of multiple polygon overlays.

class MKOverlayPathRenderer

The visual representation of a path-based overlay.

