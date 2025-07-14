

- RealityKit
- Entity
-  orientation 

Instance Property

# orientation

The rotation of the entity relative to its parent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var orientation: simd_quatf { get set }
```

## Discussion

This value is the entity’s rotation relative to its parent. To get the world-space orientation of the entity, use orientation(relativeTo:), passing `nil` as the reference entity.

This is the same as the rotation value on the transform.

