

- ARKit
- ARRaycastResult
-  worldTransform 

Instance Property

# worldTransform

The position, rotation, and scale, of the ray’s intersection with the target.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var worldTransform: simd_float4x4 { get }
```

## See Also

### Identifying Results

var anchor: ARAnchor?

The anchor for the plane that the ray intersected.

var target: ARRaycastQuery.Target

The type of surface that the ray intersects.

enum Target

The types of surface you allow a raycast to intersect with.

var targetAlignment: ARRaycastQuery.TargetAlignment

The alignment of the plane that the ray intersected.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

