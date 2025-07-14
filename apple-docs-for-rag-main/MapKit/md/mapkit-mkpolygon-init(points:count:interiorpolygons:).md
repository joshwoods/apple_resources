

- MapKit
- MKPolygon
-  init(points:count:interiorPolygons:) 

Initializer

# init(points:count:interiorPolygons:)

Creates and returns a polygon object from the specified set of map points and interior polygons.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    points: UnsafePointer,
    count: Int,
    interiorPolygons: [MKPolygon]?
)
```

## Parameters 

`points`  

The array of map points defining the shape. The new object copy the data in this array.

`count`  

The number of items in the `points` array.

`interiorPolygons`  

An array of `MKPolygon` objects that define one or more cutout regions for the receiver’s polygon.

## Return Value

A new polygon object.

## See Also

### Creating a polygon overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int)

Creates and returns a polygon object from the specified set of map points.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates and returns a polygon object from the specified set of coordinates.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int, interiorPolygons: [MKPolygon]?)

Creates and returns a polygon object from the specified set of coordinates and interior polygons.

