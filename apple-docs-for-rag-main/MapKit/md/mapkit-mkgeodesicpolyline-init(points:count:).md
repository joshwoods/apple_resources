

- MapKit
- MKGeodesicPolyline
-  init(points:count:) 

Initializer

# init(points:count:)

Creates and returns a geodesic polyline using the specified map points.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    points: UnsafePointer,
    count: Int
)
```

## Parameters 

`points`  

A pointer to the array of map points that define the path.

`count`  

The number of items in the `points` array.

## Return Value

A new geodesic polyline object.

## See Also

### Creating a geodesic polyline overlay

convenience init(coordinates: UnsafePointer&lt;CLLocationCoordinate2D>, count: Int)

Creates and returns a geodesic polyline using the specified coordinates.

