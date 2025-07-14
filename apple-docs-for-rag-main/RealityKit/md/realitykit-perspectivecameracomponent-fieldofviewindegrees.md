

- RealityKit
- PerspectiveCameraComponent
-  fieldOfViewInDegrees 

Instance Property

# fieldOfViewInDegrees

The camera’s total field of view in degrees.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var fieldOfViewInDegrees: Float
```

## Discussion

This property contains the entire field of view for the camera in degrees.

When you set fieldOfViewOrientation to CameraFieldOfViewOrientation.vertical, this value sets the vertical field of view for the camera in degrees, and the system automatically calculates the horizontal field of view to fit the aspect ratio of the device’s screen.

This property defaults to `60` degrees.

## See Also

### Setting the field of view

var fieldOfViewOrientation: CameraFieldOfViewOrientation

The orientation with which the system uses to apply the field-of-view degrees.

