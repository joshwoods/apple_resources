

- ARKit
- ARHitTestResult
-  worldTransform Deprecated

Instance Property

# worldTransform

The position and orientation of the result relative to the world coordinate system.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
var worldTransform: simd_float4x4 { get }
```

Deprecated

Use raycasting

## Discussion

This transform matrix indicates the intersection point between the detected surface and the ray that created the hit-test result. A hit-test projects a 2D point in the image or view coordinate system along a ray into the 3D world space and reports results where that line intersects detected surfaces.

The session configuration’s worldAlignment property defines the world coordinate system.

## See Also

### Examining Result Geometry

var distance: CGFloat

The distance, in meters, from the camera to the detected surface.

Deprecated

var localTransform: simd_float4x4

The position and orientation of the result relative to the nearest anchor or feature point.

Deprecated

