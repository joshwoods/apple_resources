

- MapKit
- MKMapView
-  MKMapView.CameraZoomRange 

Class

# MKMapView.CameraZoomRange

A camera zoom range that limits the distances to which the user can zoom.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class CameraZoomRange
```

## Overview

Create a camera zoom range to limit the distance to which the user can zoom. After you create the camera zoom range, you can apply it to multiple map views. If you don’t create a camera zoom range, your map view allows the user to zoom to MapKit’s capabilities.

## Topics

### Creating a camera zoom range

init?(minCenterCoordinateDistance: CLLocationDistance, maxCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying a minimum and maximum distance from your map view’s center coordinates, measured in meters.

convenience init?(minCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying the minimum distance from your map view’s center coordinate, measured in meters.

convenience init?(maxCenterCoordinateDistance: CLLocationDistance)

Create a camera zoom range by specifying the maximum distance from your map view’s center coordinate, measured in meters.

let MKMapCameraZoomDefault: CLLocationDistance

A constant value used to represent the default value for zooming in or out on a map.

### Accessing zoom range values

var maxCenterCoordinateDistance: CLLocationDistance

The maximum distance of the camera to the center of the map, measured in meters.

var minCenterCoordinateDistance: CLLocationDistance

The minimum distance of the camera to the center of the map, measured in meters.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Constraining the map view

func setCameraBoundary(MKMapView.CameraBoundary?, animated: Bool)

Sets the camera boundary for the map view, specifying whether to use animation.

var cameraBoundary: MKMapView.CameraBoundary?

The boundary of the area within which the map view’s center needs to remain.

func setCameraZoomRange(MKMapView.CameraZoomRange?, animated: Bool)

Sets the camera zoom range for the map view, specifying whether to use animation.

var cameraZoomRange: MKMapView.CameraZoomRange!

The zoom range to apply to the map view.

class CameraBoundary

A boundary of an area within which the map’s center needs to remain.

