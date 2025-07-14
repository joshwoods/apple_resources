

- RealityKit
- HasTransform
-  position 

Instance Property

# position

The position of the entity relative to its parent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var position: SIMD3 { get set }
```

## Discussion

This value is the entity’s position relative to its parent. To get the world-space position of the entity in the scene, use position(relativeTo:), passing `nil` as the reference entity.

This is the same as the translation value on the transform.

## See Also

### Positioning an entity

func position(relativeTo: Entity?) -> SIMD3&lt;Float>

Gets the position of an entity relative to the given entity.

func setPosition(SIMD3&lt;Float>, relativeTo: Entity?)

Sets the position of the entity relative to the given reference entity.

