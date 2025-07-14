

- MapKit
- MKMapView
-  MKMapView.CameraBoundary 

Class

# MKMapView.CameraBoundary

A boundary of an area within which the map’s center needs to remain.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class CameraBoundary
```

## Overview

The constraints of the camera boundary restrict the center point of your map.

## Topics

### Creating a camera boundary

init?(coder: NSCoder)

Creates a camera boundary using the provided coder.

init?(coordinateRegion: MKCoordinateRegion)

Creates a camera boundary using the provided coordinate region.

init?(mapRect: MKMapRect)

Creates a camera boundary using the provided map rectangle.

### Accessing the boundary

var mapRect: MKMapRect

The map rectangle that describes the camera boundary.

var region: MKCoordinateRegion

The coordinate region that describes the camera boundary.

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

class CameraZoomRange

A camera zoom range that limits the distances to which the user can zoom.

