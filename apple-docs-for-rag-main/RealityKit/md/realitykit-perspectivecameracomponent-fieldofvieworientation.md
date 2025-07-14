

- RealityKit
- PerspectiveCameraComponent
-  fieldOfViewOrientation 

Instance Property

# fieldOfViewOrientation

The orientation with which the system uses to apply the field-of-view degrees.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var fieldOfViewOrientation: CameraFieldOfViewOrientation
```

## Discussion

The value of this property determines the orientation that the system uses to apply the fieldOfViewInDegrees value.

This property defaults to CameraFieldOfViewOrientation.vertical.

## See Also

### Setting the field of view

var fieldOfViewInDegrees: Float

The camera’s total field of view in degrees.

