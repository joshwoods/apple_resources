

- ARKit
- ARRaycastResult
-  targetAlignment 

Instance Property

# targetAlignment

The alignment of the plane that the ray intersected.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var targetAlignment: ARRaycastQuery.TargetAlignment { get }
```

## See Also

### Identifying Results

var worldTransform: simd_float4x4

The position, rotation, and scale, of the ray’s intersection with the target.

var anchor: ARAnchor?

The anchor for the plane that the ray intersected.

var target: ARRaycastQuery.Target

The type of surface that the ray intersects.

enum Target

The types of surface you allow a raycast to intersect with.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

