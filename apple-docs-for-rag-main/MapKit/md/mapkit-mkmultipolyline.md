

- MapKit
-  MKMultiPolyline 

Class

# MKMultiPolyline

A collection of multipolyline shapes, each consisting of one or more connected line segments.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MKMultiPolyline
```

## Overview

Use a MKMultiPolyline object when you have multiple distinct polyline shapes that you intend to render using the same style.

## Topics

### Creating a multipolyline object

init([MKPolyline])

Creates a multipolyline object using the provided polylines.

### Accessing polyline objects

var polylines: [MKPolyline]

An array containing the polyline objects that make up the multipolyline object.

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

### Multiple segment lines

class MKPolyline

An open polygon overlay consisting of one or more connected line segments.

class MKGeodesicPolyline

An open polygon overlay consisting of line segments that follow the contours of the Earth to create the shortest path between the specified points.

class MKPolylineRenderer

A visual representation of any polyline overlay object.

class MKMultiPolylineRenderer

A visual representation of multiple polyline overlay objects.

class MKGradientPolylineRenderer

A visual representation of any polyline overlay object with a gradient.

