

- MapKit
- MKPolyline
-  init(points:count:) 

Initializer

# init(points:count:)

Creates a polyline object from the specified set of map points.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    points: UnsafePointer,
    count: Int
)
```

## Parameters 

`points`  

The array of map points defining the shape. The initializer copies the data in this array to the new object.

`count`  

The number of items in the `points` array.

## Return Value

A new polyline object.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a polyline overlay

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates a polyline object from the specified set of coordinates.

