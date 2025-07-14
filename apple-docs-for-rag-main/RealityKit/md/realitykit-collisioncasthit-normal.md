

- RealityKit
- CollisionCastHit
-  normal 

Instance Property

# normal

The normal of the hit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var normal: SIMD3 { get }
```

## Discussion

The frame of reference for this point depends on the reference entity used in the call to either the raycast(origin:direction:length:query:mask:relativeTo:) method or the convexCast(convexShape:fromPosition:fromOrientation:toPosition:toOrientation:query:mask:relativeTo:) method that generated the hit.

## See Also

### Characterizing the collision cast hit

var position: SIMD3&lt;Float>

The position of the hit.

var distance: Float

The distance from the ray origin to the hit, or the convex shape travel distance.

