

- MapKit
-  MKPolylineRenderer 

Class

# MKPolylineRenderer

A visual representation of any polyline overlay object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKPolylineRenderer
```

## Overview

This renderer strokes the line only; it doesn’t fill it. You can change the color and other drawing attributes of the polyline by modifying the properties it inherits from the main class. You typically use this class as-is and don’t subclass it.

## Topics

### Creating a polyline renderer

init(polyline: MKPolyline)

Creates a new overlay view using the specified polyline overlay object.

### Accessing the polyline overlay

var polyline: MKPolyline

The polyline overlay object that contains the information for drawing the overlay.

### Accessing the stroke

var strokeStart: CGFloat

The unit distance along the line where the stroke starts.

var strokeEnd: CGFloat

The unit distance along the line where the stroke ends.

## Relationships

### Inherits From

- MKOverlayPathRenderer

### Inherited By

- MKGradientPolylineRenderer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Multiple segment lines

class MKPolyline

An open polygon overlay consisting of one or more connected line segments.

class MKGeodesicPolyline

An open polygon overlay consisting of line segments that follow the contours of the Earth to create the shortest path between the specified points.

class MKMultiPolyline

A collection of multipolyline shapes, each consisting of one or more connected line segments.

class MKMultiPolylineRenderer

A visual representation of multiple polyline overlay objects.

class MKGradientPolylineRenderer

A visual representation of any polyline overlay object with a gradient.

