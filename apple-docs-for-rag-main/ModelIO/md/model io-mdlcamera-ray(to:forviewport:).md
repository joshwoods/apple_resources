

- Model I/O
- MDLCamera
-  ray(to:forViewPort:) 

Instance Method

# ray(to:forViewPort:)

Returns a point, in 3D world coordinates, corresponding to the specified 2D view coordinates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func ray(
    to pixel: vector_int2,
    forViewPort size: vector_int2
) -> vector_float3
```

## Parameters 

`pixel`  

A point in the 2D pixel coordinate system of a possible renderer’s view.

`size`  

The pixel dimensions of a possible renderer’s view.

## Return Value

A set of 3D world coordinates.

## Discussion

This method projects a ray from the camera’s location in the direction of the specified view coordinates, returning the world coordinates where that ray intersects a plane at a distance of 1.0 units (of world coordinate space) away from the camera.

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

var worldToMetersConversionScale: Float

The scale factor to meters from the world coordinate system containing the camera.

