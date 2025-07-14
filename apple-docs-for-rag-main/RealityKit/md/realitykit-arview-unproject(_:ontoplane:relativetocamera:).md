

- RealityKit
- ARView
-  unproject(\_:ontoPlane:relativeToCamera:) 

Instance Method

# unproject(\_:ontoPlane:relativeToCamera:)

Unproject a 2D point from the view onto a plane in 3D world coordinates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
@MainActor @preconcurrency
func unproject(
    _ point: CGPoint,
    ontoPlane planeTransform: float4x4,
    relativeToCamera: Bool
) -> SIMD3?
```

## Parameters 

`point`  

A point in the view’s coordinate system.

`planeTransform`  

The transform used to define the coordinate system of the plane. The coordinate system’s positive y-axis is assumed to be the normal of the plane.

`relativeToCamera`  

If the plane transform is relative to camera space or world space.

## Return Value

3D position in world coordinates or nil if unprojection is not possible.

## Discussion

A 2D point in the view’s coordinate space can refer to any point along a line segment in the 3D coordinate space. Unprojecting gets the 3D position of the point along this line segment that intersects the provided plane.

## See Also

### Mapping between coordinate spaces

func project(SIMD3&lt;Float>) -> CGPoint?

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the view.

func unproject(CGPoint, ontoPlane: float4x4) -> SIMD3&lt;Float>?

Maps a 2D point from the view’s coordinate system onto the given plane in 3D space.

func unproject(CGPoint, viewport: CGRect) -> SIMD3&lt;Float>?

Maps a 2D point from the pixel coordinate system of a viewport into a 3D coordinate space. The point lies on this view’s near clipping plane.

func ray(through: CGPoint) -> (origin: SIMD3&lt;Float>, direction: SIMD3&lt;Float>)?

Determines the position and direction of a ray through the given point in the 2D space of the view.

