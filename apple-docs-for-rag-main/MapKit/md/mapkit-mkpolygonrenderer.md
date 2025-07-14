

- MapKit
-  MKPolygonRenderer 

Class

# MKPolygonRenderer

The visual representation of a single polygon overlay.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKPolygonRenderer
```

## Overview

This renderer creates the polygon overlay by first filling the shape and then representing its outline with strokes. You can change the color and other drawing attributes of the polygon by modifying the properties inherited from the parent class.

## Topics

### Creating a polygon renderer

init(polygon: MKPolygon)

Creates a new renderer that handles drawing for the specified polygon overlay object.

### Accessing the polygon overlay object

var polygon: MKPolygon

The polygon object that contains the information used to draw the overlay’s contents.

### Accessing the stroke

var strokeStart: CGFloat

The unit distance along the polygon where the stroke starts.

var strokeEnd: CGFloat

The unit distance along the polygon where the stroke ends.

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

class MKMultiPolygon

A collection of multiple closed polygon overlays.

class MKMultiPolygonRenderer

The visual representation of multiple polygon overlays.

class MKOverlayPathRenderer

The visual representation of a path-based overlay.

