

- MapKit
- MKMapView
-  cameraBoundary 

Instance Property

# cameraBoundary

The boundary of the area within which the map view’s center needs to remain.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var cameraBoundary: MKMapView.CameraBoundary? { get set }
```

## See Also

### Constraining the map view

func setCameraBoundary(MKMapView.CameraBoundary?, animated: Bool)

Sets the camera boundary for the map view, specifying whether to use animation.

func setCameraZoomRange(MKMapView.CameraZoomRange?, animated: Bool)

Sets the camera zoom range for the map view, specifying whether to use animation.

var cameraZoomRange: MKMapView.CameraZoomRange!

The zoom range to apply to the map view.

class CameraBoundary

A boundary of an area within which the map’s center needs to remain.

class CameraZoomRange

A camera zoom range that limits the distances to which the user can zoom.

