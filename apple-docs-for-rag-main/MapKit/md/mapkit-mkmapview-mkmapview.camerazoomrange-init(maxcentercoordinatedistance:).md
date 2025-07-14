

- MapKit
- MKMapView
- MKMapView.CameraZoomRange
-  init(maxCenterCoordinateDistance:) 

Initializer

# init(maxCenterCoordinateDistance:)

Create a camera zoom range by specifying the maximum distance from your map view’s center coordinate, measured in meters.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
convenience init?(maxCenterCoordinateDistance maxDistance: CLLocationDistance)
```

## Parameters 

`maxDistance`  

The maximum distance the user can zoom out on a map based on its center point, measured in meters.

To increase how far out the user can zoom, use a larger distance value. To decrease how far out the user can zoom, use a smaller distance value.

## Discussion

The constant, MKMapCameraZoomDefault, specifies the default distance for maxCenterCoordinateDistance.

## See Also

### Creating a camera zoom range

init?(minCenterCoordinateDistance: CLLocationDistance, maxCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying a minimum and maximum distance from your map view’s center coordinates, measured in meters.

convenience init?(minCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying the minimum distance from your map view’s center coordinate, measured in meters.

let MKMapCameraZoomDefault: CLLocationDistance

A constant value used to represent the default value for zooming in or out on a map.

