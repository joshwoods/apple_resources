

- Model I/O
-  MDLCameraProjection 

Enumeration

# MDLCameraProjection

Options for camera projection styles, used by the projection property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLCameraProjection
```

## Topics

### Constants

case orthographic

An orthographic projection.

case perspective

A perspective projection.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Camera Perspective

var projectionMatrix: matrix_float4x4

A transformation matrix that determines the extent of a scene visible to the camera.

var projection: MDLCameraProjection

The style of projection transform used by the camera.

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

