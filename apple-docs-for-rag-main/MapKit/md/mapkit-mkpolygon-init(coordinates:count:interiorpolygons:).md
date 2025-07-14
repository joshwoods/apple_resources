

- MapKit
- MKPolygon
-  init(coordinates:count:interiorPolygons:) 

Initializer

# init(coordinates:count:interiorPolygons:)

Creates and returns a polygon object from the specified set of coordinates and interior polygons.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    coordinates coords: UnsafePointer,
    count: Int,
    interiorPolygons: [MKPolygon]?
)
```

## Parameters 

`coords`  

The array of coordinates defining the shape. The new object copies the data in this array.

`count`  

The number of items in the `coords` array.

`interiorPolygons`  

An array of `MKPolygon` objects that define one or more cutout regions for the receiver’s polygon.

## Return Value

A new polygon object.

## See Also

### Creating a polygon overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int)

Creates and returns a polygon object from the specified set of map points.

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int, interiorPolygons: [MKPolygon]?)

Creates and returns a polygon object from the specified set of map points and interior polygons.

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates and returns a polygon object from the specified set of coordinates.

