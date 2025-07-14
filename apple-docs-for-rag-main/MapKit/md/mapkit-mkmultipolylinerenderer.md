

- MapKit
-  MKMultiPolylineRenderer 

Class

# MKMultiPolylineRenderer

A visual representation of multiple polyline overlay objects.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MKMultiPolylineRenderer
```

## Overview

Use the multipolyline renderer to provide the styling of multiple polylines that you create using MKMultiPolyline.

## Topics

### Creating a multipolyline renderer

init(multiPolyline: MKMultiPolyline)

Creates an object that renders a visual representation of multiple polyline objects.

### Accessing the multipolyline object

var multiPolyline: MKMultiPolyline

An object that represents multiple polyline shapes, each consisting of one or more connected line segments.

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

### Multiple segment lines

class MKPolyline

An open polygon overlay consisting of one or more connected line segments.

class MKGeodesicPolyline

An open polygon overlay consisting of line segments that follow the contours of the Earth to create the shortest path between the specified points.

class MKMultiPolyline

A collection of multipolyline shapes, each consisting of one or more connected line segments.

class MKPolylineRenderer

A visual representation of any polyline overlay object.

class MKGradientPolylineRenderer

A visual representation of any polyline overlay object with a gradient.

