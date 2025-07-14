

- MapKit
- MKMapView
-  cameraZoomRange 

Instance Property

# cameraZoomRange

The zoom range to apply to the map view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var cameraZoomRange: MKMapView.CameraZoomRange! { get set }
```

## See Also

### Constraining the map view

func setCameraBoundary(MKMapView.CameraBoundary?, animated: Bool)

Sets the camera boundary for the map view, specifying whether to use animation.

var cameraBoundary: MKMapView.CameraBoundary?

The boundary of the area within which the map view’s center needs to remain.

func setCameraZoomRange(MKMapView.CameraZoomRange?, animated: Bool)

Sets the camera zoom range for the map view, specifying whether to use animation.

class CameraBoundary

A boundary of an area within which the map’s center needs to remain.

class CameraZoomRange

A camera zoom range that limits the distances to which the user can zoom.

