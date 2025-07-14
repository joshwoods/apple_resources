

- MapKit
- MKMapView
- MKMapView.CameraZoomRange
-  init(minCenterCoordinateDistance:) 

Initializer

# init(minCenterCoordinateDistance:)

Create a camera zoom range by specifying the minimum distance from your map view’s center coordinate, measured in meters.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
convenience init?(minCenterCoordinateDistance minDistance: CLLocationDistance)
```

## Parameters 

`minDistance`  

The minimum distance the user can zoom in on a map based on its center point, measured in meters.

To increase how far in the user can zoom, use a shorter distance value. To decrease how far in the user can zoom, use a larger distance value.

## Discussion

To specify MapKit’s default minimum distance from the center coordinate, use the MKMapCameraZoomDefault constant, that allows the user to zoom to any level that MapKit supports.

The following example prevents the user from zooming closer than 1000 meters from the map’s center coordinate:

```
MKMapView.CameraZoomRange(
    minCenterCoordinateDistance: 1000
)
```

## See Also

### Creating a camera zoom range

init?(minCenterCoordinateDistance: CLLocationDistance, maxCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying a minimum and maximum distance from your map view’s center coordinates, measured in meters.

convenience init?(maxCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying the maximum distance from your map view’s center coordinate, measured in meters.

let MKMapCameraZoomDefault: CLLocationDistance

A constant value used to represent the default value for zooming in or out on a map.

