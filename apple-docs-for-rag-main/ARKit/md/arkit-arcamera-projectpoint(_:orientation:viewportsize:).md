

- ARKit
- ARCamera
-  projectPoint(\_:orientation:viewportSize:) 

Instance Method

# projectPoint(\_:orientation:viewportSize:)

Returns the projection of a point from the 3D world space detected by ARKit into the 2D space of a view rendering the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func projectPoint(
    _ point: simd_float3,
    orientation: UIInterfaceOrientation,
    viewportSize: CGSize
) -> CGPoint
```

## Parameters 

`point`  

The 3D world-space point to project into 2D view space.

`orientation`  

The orientation in which the camera image is to be presented.

`viewportSize`  

The size, in points, of the view in which the camera image is to be presented.

## Return Value

The projection of the specified point into a 2D pixel coordinate space whose origin is in the upper left corner and whose size matches that of the `viewportSize` parameter.

## Discussion

If you display AR content with SceneKit, the ARSCNView class provides an otherwise equivalent projectPoint(_:) method that requires fewer parameters (because the view can infer its orientation and size).

## See Also

### Applying Camera Geometry

var projectionMatrix: simd_float4x4

A transform matrix appropriate for rendering 3D content to match the image captured by the camera.

func projectionMatrix(for: UIInterfaceOrientation, viewportSize: CGSize, zNear: CGFloat, zFar: CGFloat) -> simd_float4x4

Returns a transform matrix appropriate for rendering 3D content to match the image captured by the camera, using the specified parameters.

func viewMatrix(for: UIInterfaceOrientation) -> simd_float4x4

Returns a transform matrix for converting from world space to camera space.

func unprojectPoint(CGPoint, ontoPlane: simd_float4x4, orientation: UIInterfaceOrientation, viewportSize: CGSize) -> simd_float3?

Returns the projection of a point from the 2D space of a view rendering the scene onto a plane in the 3D world space detected by ARKit.

