

- MapKit
-  MKPolyline 

Class

# MKPolyline

An open polygon overlay consisting of one or more connected line segments.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKPolyline
```

## Overview

The points connect end-to-end in the order that you provide them. The first and last points don’t automatically connect to each other.

## Topics

### Creating a polyline overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int)

Creates a polyline object from the specified set of map points.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates a polyline object from the specified set of coordinates.

## Relationships

### Inherits From

- MKMultiPoint

### Inherited By

- MKGeodesicPolyline

### Conforms To

- CVarArg
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

class MKGeodesicPolyline

An open polygon overlay consisting of line segments that follow the contours of the Earth to create the shortest path between the specified points.

class MKMultiPolyline

A collection of multipolyline shapes, each consisting of one or more connected line segments.

class MKPolylineRenderer

A visual representation of any polyline overlay object.

class MKMultiPolylineRenderer

A visual representation of multiple polyline overlay objects.

class MKGradientPolylineRenderer

A visual representation of any polyline overlay object with a gradient.

