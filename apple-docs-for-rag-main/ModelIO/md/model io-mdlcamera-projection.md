

- Model I/O
- MDLCamera
-  projection 

Instance Property

# projection

The style of projection transform used by the camera.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var projection: MDLCameraProjection { get set }
```

## Discussion

A renderer can use this information to change its interpretation or recalculation of the projectionMatrix property.

## See Also

### Managing Camera Perspective

var projectionMatrix: matrix_float4x4

A transformation matrix that determines the extent of a scene visible to the camera.

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

var worldToMetersConversionScale: Float

The scale factor to meters from the world coordinate system containing the camera.

