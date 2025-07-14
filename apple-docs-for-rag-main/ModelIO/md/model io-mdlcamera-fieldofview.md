

- Model I/O
- MDLCamera
-  fieldOfView 

Instance Property

# fieldOfView

The camera’s field of view, in degrees.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var fieldOfView: Float { get set }
```

## Discussion

Field of view is an angle that determines the extent of the scene visible to the camera. A small field of view angle provides a narrow view, and a large field of view provides a wide view. A very wide field of view results in distorted perspective.

In a physically based camera, field of view is based on the focal length of the lens and the vertical aperture of the imaging surface (film or sensor). Changing the focalLength or sensorVerticalAperture property updates the fieldOfView property to the corresponding value, and vice versa.

The default field of view is 54 degrees, corresponding to a focal length of 50mm and a vertical sensor aperture of 24mm.

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

func ray(to: vector_int2, forViewPort: vector_int2) -> vector_float3

Returns a point, in 3D world coordinates, corresponding to the specified 2D view coordinates.

var worldToMetersConversionScale: Float

The scale factor to meters from the world coordinate system containing the camera.

