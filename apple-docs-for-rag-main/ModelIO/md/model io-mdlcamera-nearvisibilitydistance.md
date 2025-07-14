

- Model I/O
- MDLCamera
-  nearVisibilityDistance 

Instance Property

# nearVisibilityDistance

The camera’s near depth limit.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var nearVisibilityDistance: Float { get set }
```

## Discussion

The near value determines the minimal distance between the camera and a visible surface. If a surface is closer to the camera than this distance, the surface is clipped and does not appear.

## See Also

### Managing Camera Perspective

var projectionMatrix: matrix_float4x4

A transformation matrix that determines the extent of a scene visible to the camera.

var projection: MDLCameraProjection

The style of projection transform used by the camera.

enum MDLCameraProjection

Options for camera projection styles, used by the projection property.

var farVisibilityDistance: Float

The camera’s far depth limit.

var fieldOfView: Float

The camera’s field of view, in degrees.

func ray(to: vector_int2, forViewPort: vector_int2) -> vector_float3

Returns a point, in 3D world coordinates, corresponding to the specified 2D view coordinates.

var worldToMetersConversionScale: Float

The scale factor to meters from the world coordinate system containing the camera.

