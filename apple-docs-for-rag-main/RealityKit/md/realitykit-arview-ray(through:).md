

- RealityKit
- ARView
-  ray(through:) 

Instance Method

# ray(through:)

Determines the position and direction of a ray through the given point in the 2D space of the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
func ray(through screenPoint: CGPoint) -> (origin: SIMD3, direction: SIMD3)?
```

## Parameters 

`screenPoint`  

A point in the view’s coordinate system.

## Return Value

A tuple that represents a ray in AR coordinates that goes from the camera origin through the specified point on the screen.

## See Also

### Mapping between coordinate spaces

func project(SIMD3&lt;Float>) -> CGPoint?

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the view.

func unproject(CGPoint, ontoPlane: float4x4, relativeToCamera: Bool) -> SIMD3&lt;Float>?

Unproject a 2D point from the view onto a plane in 3D world coordinates.

func unproject(CGPoint, ontoPlane: float4x4) -> SIMD3&lt;Float>?

Maps a 2D point from the view’s coordinate system onto the given plane in 3D space.

func unproject(CGPoint, viewport: CGRect) -> SIMD3&lt;Float>?

Maps a 2D point from the pixel coordinate system of a viewport into a 3D coordinate space. The point lies on this view’s near clipping plane.

