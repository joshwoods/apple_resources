

- Model I/O
- MDLCamera
-  frameBoundingBox(\_:setNearAndFar:) 

Instance Method

# frameBoundingBox(\_:setNearAndFar:)

Moves the camera such that the specified bounding box lies entirely within the camera’s field of view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func frameBoundingBox(
    _ boundingBox: MDLAxisAlignedBoundingBox,
    setNearAndFar: Bool
)
```

## Parameters 

`boundingBox`  

The region, in world space coordinates, to be made visible to the camera.

`setNearAndFar`  

If true, the camera also adjusts its nearVisibilityDistance and farVisibilityDistance properties to place the specified region entirely within the camera’s viewing frustum. If false, those properties remain unchanged, and the specified region may therefore lie outside the camera’s near and far limits.

## Discussion

When calculating the new camera position and orientation, this method assumes the camera points in the negative z-axis direction and that the positive y-axis represents the up direction for the camera’s view.

## See Also

### Managing Camera Position and Orientation

func look(at: vector_float3)

Orients the camera to face toward the specified point.

func look(at: vector_float3, from: vector_float3)

Sets the camera’s position and orients the camera to face toward the specified point.

