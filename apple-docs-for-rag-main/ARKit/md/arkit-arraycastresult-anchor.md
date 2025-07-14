

- ARKit
- ARRaycastResult
-  anchor 

Instance Property

# anchor

The anchor for the plane that the ray intersected.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var anchor: ARAnchor? { get }
```

## Discussion

If you chose an existing plane target, ARKit provides its anchor. If you choose an estimated plane target, ARKit provides an anchor only if the ray intersects an existing plane.

## See Also

### Identifying Results

var worldTransform: simd_float4x4

The position, rotation, and scale, of the ray’s intersection with the target.

var target: ARRaycastQuery.Target

The type of surface that the ray intersects.

enum Target

The types of surface you allow a raycast to intersect with.

var targetAlignment: ARRaycastQuery.TargetAlignment

The alignment of the plane that the ray intersected.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

