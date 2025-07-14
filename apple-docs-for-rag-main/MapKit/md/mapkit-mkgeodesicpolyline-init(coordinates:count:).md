

- MapKit
- MKGeodesicPolyline
-  init(coordinates:count:) 

Initializer

# init(coordinates:count:)

Creates and returns a geodesic polyline using the specified coordinates.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    coordinates coords: UnsafePointer,
    count: Int
)
```

## Parameters 

`coords`  

A pointer to the array of coordinates that define the path.

`count`  

The number of items in the `coords` array.

## Return Value

A new geodesic polyline object.

## See Also

### Creating a geodesic polyline overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int)

Creates and returns a geodesic polyline using the specified map points.

