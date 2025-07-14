

- RealityKit
- PerspectiveCameraComponent
-  init(near:far:fieldOfViewInDegrees:) 

Initializer

# init(near:far:fieldOfViewInDegrees:)

Creates a perspective camera component from near and far clipping planes and a field of view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init(
    near: Float = 0.01,
    far: Float = .infinity,
    fieldOfViewInDegrees: Float = 60.0
)
```

## Parameters 

`near`  

The minimum distance in meters from the camera that the camera can see.

`far`  

The maximum distance in meters from the camera that the camera can see.

`fieldOfViewInDegrees`  

The camera’s field of view, in degrees.

## See Also

### Creating a camera component

init(near: Float, far: Float, fieldOfViewInDegrees: Float, fieldOfViewOrientation: CameraFieldOfViewOrientation)

Creates a perspective camera component from near and far clipping planes, a field of view, and an orientation.

