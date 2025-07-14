

- MapKit
-  MKMapCameraZoomDefault 

Global Variable

# MKMapCameraZoomDefault

A constant value used to represent the default value for zooming in or out on a map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
let MKMapCameraZoomDefault: CLLocationDistance
```

## Discussion

Use MKMapCameraZoomDefault for the minimum or maximum zoom range when you create an instance of MKMapView.CameraZoomRange to allow the user to zoom to any level that MapKit supports.

## See Also

### Creating a camera zoom range

init?(minCenterCoordinateDistance: CLLocationDistance, maxCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying a minimum and maximum distance from your map view’s center coordinates, measured in meters.

convenience init?(minCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying the minimum distance from your map view’s center coordinate, measured in meters.

convenience init?(maxCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying the maximum distance from your map view’s center coordinate, measured in meters.

