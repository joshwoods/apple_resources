

- ARKit
- ARCamera
-  viewMatrix(for:) 

Instance Method

# viewMatrix(for:)

Returns a transform matrix for converting from world space to camera space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func viewMatrix(for orientation: UIInterfaceOrientation) -> simd_float4x4
```

## Parameters 

`orientation`  

The orientation in which the camera image is to be presented.

## Return Value

A view matrix appropriate for the camera with the specified orientation.

## Discussion

This method has no effect on ARKit. Instead, this method uses the orientation parameter and the camera’s state to construct a view matrix for your own rendering code.

## See Also

### Applying Camera Geometry

var projectionMatrix: simd_float4x4

A transform matrix appropriate for rendering 3D content to match the image captured by the camera.

func projectionMatrix(for: UIInterfaceOrientation, viewportSize: CGSize, zNear: CGFloat, zFar: CGFloat) -> simd_float4x4

Returns a transform matrix appropriate for rendering 3D content to match the image captured by the camera, using the specified parameters.

func projectPoint(simd_float3, orientation: UIInterfaceOrientation, viewportSize: CGSize) -> CGPoint

Returns the projection of a point from the 3D world space detected by ARKit into the 2D space of a view rendering the scene.

func unprojectPoint(CGPoint, ontoPlane: simd_float4x4, orientation: UIInterfaceOrientation, viewportSize: CGSize) -> simd_float3?

Returns the projection of a point from the 2D space of a view rendering the scene onto a plane in the 3D world space detected by ARKit.

