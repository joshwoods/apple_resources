

- MapKit
- MKPolyline
-  init(coordinates:count:) 

Initializer

# init(coordinates:count:)

Creates a polyline object from the specified set of coordinates.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    coordinates coords: UnsafePointer,
    count: Int
)
```

## Parameters 

`coords`  

The array of coordinates defining the shape. The initializer copies the data in this array to the new object.

`count`  

The number of items in the `coords` array.

## Return Value

A new polyline object.

## See Also

### Creating a polyline overlay

convenience init(points: UnsafePointer&lt;MKMapPoint>, count: Int)

Creates a polyline object from the specified set of map points.

