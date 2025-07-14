

- MapKit
-  MKMultiPoint 

Class

# MKMultiPoint

An abstract class that defines the common behavior that open and closed polygon overlays share.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class MKMultiPoint
```

## Overview

Don’t create instances of this class directly. Instead, create instances of the MKPolygon or MKPolyline classes. However, you can use the methods and property of this class to access information about the specific points associated with the line or polygon.

## Topics

### Accessing the points in the shape

func points() -> UnsafeMutablePointer&lt;MKMapPoint>

Returns an array of map points associated with the shape.

var pointCount: Int

The number of points associated with the shape.

func location(atPointIndex: Int) -> CGFloat

Translates a point index into a unit distance along the shape.

func locations(at: IndexSet) -> [CGFloat]

Translates a point index set into a unit distance along the shape.

### Getting coordinate values

func getCoordinates(UnsafeMutablePointer&lt;CLLocationCoordinate2D>, range: NSRange)

Retrieves one or more points associated with the shape and converts them to coordinate values.

## Relationships

### Inherits From

- MKShape

### Inherited By

- MKPolygon
- MKPolyline

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MKAnnotation
- MKGeoJSONObject
- NSObjectProtocol

## See Also

### Shared behavior

protocol MKOverlay

An interface for associating content with a specific map region.

class MKOverlayRenderer

The shared infrastructure for drawing overlays on the map surface.

class MKShape

An abstract class that defines the basic properties for all shape-based overlay objects.

class MKPlacemark

A user-friendly description of a location on the map.

