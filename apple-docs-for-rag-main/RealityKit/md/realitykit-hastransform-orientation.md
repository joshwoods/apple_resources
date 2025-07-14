

- RealityKit
- HasTransform
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

## See Also

### Rotating an entity

func orientation(relativeTo: Entity?) -> simd_quatf

Gets the orientation of an entity relative to the given entity.

func setOrientation(simd_quatf, relativeTo: Entity?)

Sets the orientation of the entity relative to the given reference entity.

