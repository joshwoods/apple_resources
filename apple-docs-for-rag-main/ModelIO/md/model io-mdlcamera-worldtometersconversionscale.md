

- Model I/O
- MDLCamera
-  worldToMetersConversionScale 

Instance Property

# worldToMetersConversionScale

The scale factor to meters from the world coordinate system containing the camera.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var worldToMetersConversionScale: Float { get set }
```

## Discussion

Some calculations, such as the calculation of MDLStereoscopicCamera view matrices, must occur in world space. MDLCamera properties measured in meters or millimeters use this conversion scale to perform the calculation.

The default value is 1.0.

## See Also

### Managing Camera Perspective

var projectionMatrix: matrix_float4x4

A transformation matrix that determines the extent of a scene visible to the camera.

var projection: MDLCameraProjection

The style of projection transform used by the camera.

enum MDLCameraProjection

Options for camera projection styles, used by the projection property.

var nearVisibilityDistance: Float

The camera’s near depth limit.

var farVisibilityDistance: Float

The camera’s far depth limit.

var fieldOfView: Float

The camera’s field of view, in degrees.

func ray(to: vector_int2, forViewPort: vector_int2) -> vector_float3

Returns a point, in 3D world coordinates, corresponding to the specified 2D view coordinates.

