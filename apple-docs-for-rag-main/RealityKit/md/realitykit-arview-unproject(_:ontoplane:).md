

- RealityKit
- ARView
-  unproject(\_:ontoPlane:) 

Instance Method

# unproject(\_:ontoPlane:)

Maps a 2D point from the view’s coordinate system onto the given plane in 3D space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
func unproject(
    _ point: CGPoint,
    ontoPlane planeTransform: float4x4
) -> SIMD3?
```

## Parameters 

`point`  

The point in the view’s coordinate system.

`planeTransform`  

A transform used to define the coordinate system of the plane. The positive y-axis is taken as the normal of the plane.

## Return Value

The 3D position in world coordinates, or `nil` if the mapping isn’t possible.

## See Also

### Mapping between coordinate spaces

func project(SIMD3&lt;Float>) -> CGPoint?

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the view.

func unproject(CGPoint, ontoPlane: float4x4, relativeToCamera: Bool) -> SIMD3&lt;Float>?

Unproject a 2D point from the view onto a plane in 3D world coordinates.

func unproject(CGPoint, viewport: CGRect) -> SIMD3&lt;Float>?

Maps a 2D point from the pixel coordinate system of a viewport into a 3D coordinate space. The point lies on this view’s near clipping plane.

func ray(through: CGPoint) -> (origin: SIMD3&lt;Float>, direction: SIMD3&lt;Float>)?

Determines the position and direction of a ray through the given point in the 2D space of the view.

