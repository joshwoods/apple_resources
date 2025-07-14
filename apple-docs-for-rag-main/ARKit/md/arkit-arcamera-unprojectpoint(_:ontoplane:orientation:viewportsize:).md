

- ARKit
- ARCamera
-  unprojectPoint(\_:ontoPlane:orientation:viewportSize:) 

Instance Method

# unprojectPoint(\_:ontoPlane:orientation:viewportSize:)

Returns the projection of a point from the 2D space of a view rendering the scene onto a plane in the 3D world space detected by ARKit.

iOS 12.0+iPadOS 12.0+

``` source
@nonobjc
func unprojectPoint(
    _ point: CGPoint,
    ontoPlane planeTransform: simd_float4x4,
    orientation: UIInterfaceOrientation,
    viewportSize: CGSize
) -> simd_float3?
```

## Parameters 

`point`  

The point in 2D view space to project onto a plane.

The coordinate space for this point has its origin is in the upper left corner and a size matching the `viewportSize` parameter.

`planeTransform`  

A transform matrix specifying the position and orientation of a plane (with infinite extent) in 3D world space. The plane is the xz-plane of the local coordinate space this transform defines.

`orientation`  

The orientation in which the camera image is to be presented.

`viewportSize`  

The size, in points, of the view in which the camera image is to be presented.

## Return Value

The 3D point in world space where a ray projected from the specified 2D point intersects the specified plane, or `nil` if the ray does not intersect the plane.

## Discussion

If you display AR content with SceneKit, the ARSCNView class provides an otherwise equivalent unprojectPoint(_:ontoPlane:) method that requires fewer parameters (because the view can infer its orientation and size).

## See Also

### Applying Camera Geometry

var projectionMatrix: simd_float4x4

A transform matrix appropriate for rendering 3D content to match the image captured by the camera.

func projectionMatrix(for: UIInterfaceOrientation, viewportSize: CGSize, zNear: CGFloat, zFar: CGFloat) -> simd_float4x4

Returns a transform matrix appropriate for rendering 3D content to match the image captured by the camera, using the specified parameters.

func viewMatrix(for: UIInterfaceOrientation) -> simd_float4x4

Returns a transform matrix for converting from world space to camera space.

func projectPoint(simd_float3, orientation: UIInterfaceOrientation, viewportSize: CGSize) -> CGPoint

Returns the projection of a point from the 3D world space detected by ARKit into the 2D space of a view rendering the scene.

