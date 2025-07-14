

- MapKit
-  MKGeodesicPolyline 

Class

# MKGeodesicPolyline

An open polygon overlay consisting of line segments that follow the contours of the Earth to create the shortest path between the specified points.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKGeodesicPolyline
```

## Overview

A geodesic polyline contains a set of points that connect end-to-end in the order that you provide them. The first and last points don’t automatically connect to each other. When displaying on a two-dimensional map view, the line segment between any two points may appear curved.

## Topics

### Creating a geodesic polyline overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int)

Creates and returns a geodesic polyline using the specified map points.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates and returns a geodesic polyline using the specified coordinates.

## Relationships

### Inherits From

- MKPolyline

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

class MKPolyline

An open polygon overlay consisting of one or more connected line segments.

class MKMultiPolyline

A collection of multipolyline shapes, each consisting of one or more connected line segments.

class MKPolylineRenderer

A visual representation of any polyline overlay object.

class MKMultiPolylineRenderer

A visual representation of multiple polyline overlay objects.

class MKGradientPolylineRenderer

A visual representation of any polyline overlay object with a gradient.

