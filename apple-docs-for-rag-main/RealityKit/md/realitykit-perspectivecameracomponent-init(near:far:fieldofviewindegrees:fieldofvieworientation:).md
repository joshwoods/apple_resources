

- RealityKit
- PerspectiveCameraComponent
-  init(near:far:fieldOfViewInDegrees:fieldOfViewOrientation:) 

Initializer

# init(near:far:fieldOfViewInDegrees:fieldOfViewOrientation:)

Creates a perspective camera component from near and far clipping planes, a field of view, and an orientation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    near: Float = 0.01,
    far: Float = .infinity,
    fieldOfViewInDegrees: Float = 60.0,
    fieldOfViewOrientation: CameraFieldOfViewOrientation = .vertical
)
```

## Parameters 

`near`  

The minimum distance in meters from the camera that the camera can see.

`far`  

The maximum distance in meters from the camera that the camera can see.

`fieldOfViewInDegrees`  

The camera’s field of view in degrees.

`fieldOfViewOrientation`  

The orientation of the field of view.

## See Also

### Creating a camera component

init(near: Float, far: Float, fieldOfViewInDegrees: Float)

Creates a perspective camera component from near and far clipping planes and a field of view.

