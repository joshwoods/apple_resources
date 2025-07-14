

- MapKit
- MKMapView
-  setCameraBoundary(\_:animated:) 

Instance Method

# setCameraBoundary(\_:animated:)

Sets the camera boundary for the map view, specifying whether to use animation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func setCameraBoundary(
    _ cameraBoundary: MKMapView.CameraBoundary?,
    animated: Bool
)
```

## Parameters 

`cameraBoundary`  

The new MKMapView.CameraBoundary.

`animated`  

A Boolean value that indicates whether the framework animates the transition of the map view to the new boundary.

## See Also

### Constraining the map view

var cameraBoundary: MKMapView.CameraBoundary?

The boundary of the area within which the map view’s center needs to remain.

func setCameraZoomRange(MKMapView.CameraZoomRange?, animated: Bool)

Sets the camera zoom range for the map view, specifying whether to use animation.

var cameraZoomRange: MKMapView.CameraZoomRange!

The zoom range to apply to the map view.

class CameraBoundary

A boundary of an area within which the map’s center needs to remain.

class CameraZoomRange

A camera zoom range that limits the distances to which the user can zoom.

