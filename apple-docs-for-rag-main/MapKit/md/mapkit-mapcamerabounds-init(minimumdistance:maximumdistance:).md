

- MapKit
- MapCameraBounds
-  init(minimumDistance:maximumDistance:) 

Initializer

# init(minimumDistance:maximumDistance:)

Creates a camera bounds with the zoom ranges you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    minimumDistance: Double? = nil,
    maximumDistance: Double? = nil
)
```

## Parameters 

`minimumDistance`  

The minimum distance someone can zoom in on a map based on its center point, measured in meters.

`maximumDistance`  

The maximum distance someone can zoom out on a map based on its center point, measured in meters.

## See Also

### Creating a map camera bounds

init(centerCoordinateBounds: MKCoordinateRegion, minimumDistance: Double?, maximumDistance: Double?)

Creates a camera bounds with the specified region boundary and zoom ranges.

init(centerCoordinateBounds: MKMapRect, minimumDistance: Double?, maximumDistance: Double?)

Creates a camera bounds with the specified map rectangle boundary and zoom ranges.

