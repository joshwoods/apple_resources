

- MapKit
- MapCameraBounds
-  init(centerCoordinateBounds:minimumDistance:maximumDistance:) 

Initializer

# init(centerCoordinateBounds:minimumDistance:maximumDistance:)

Creates a camera bounds with the specified region boundary and zoom ranges.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    centerCoordinateBounds: MKCoordinateRegion,
    minimumDistance: Double? = nil,
    maximumDistance: Double? = nil
)
```

## Parameters 

`centerCoordinateBounds`  

A boundary of an area within which the map’s center needs to remain.

`minimumDistance`  

The minimum distance someone can zoom in on a map based on its center point, measured in meters.

`maximumDistance`  

The maximum distance someone can zoom out on a map based on its center point, measured in meters.

## See Also

### Creating a map camera bounds

init(centerCoordinateBounds: MKMapRect, minimumDistance: Double?, maximumDistance: Double?)

Creates a camera bounds with the specified map rectangle boundary and zoom ranges.

init(minimumDistance: Double?, maximumDistance: Double?)

Creates a camera bounds with the zoom ranges you specify.

