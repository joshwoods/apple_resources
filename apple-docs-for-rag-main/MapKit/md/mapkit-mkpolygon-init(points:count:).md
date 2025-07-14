

- MapKit
- MKPolygon
-  init(points:count:) 

Initializer

# init(points:count:)

Creates and returns a polygon object from the specified set of map points.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    points: UnsafePointer,
    count: Int
)
```

## Parameters 

`points`  

The array of map points defining the shape. The new object copy the data in this array.

`count`  

The number of items in the `points` array.

## Return Value

A new polygon object.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a polygon overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int, interiorPolygons: [MKPolygon]?)

Creates and returns a polygon object from the specified set of map points and interior polygons.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates and returns a polygon object from the specified set of coordinates.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int, interiorPolygons: [MKPolygon]?)

Creates and returns a polygon object from the specified set of coordinates and interior polygons.

