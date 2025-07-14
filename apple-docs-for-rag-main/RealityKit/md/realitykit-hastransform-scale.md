

- RealityKit
- HasTransform
-  scale 

Instance Property

# scale

The scale of the entity relative to its parent.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var scale: SIMD3 { get set }
```

## Discussion

This value is the entity’s scale relative to its parent. To get the actual scale of the entity in the scene, use scale(relativeTo:), passing `nil` as the reference entity.

This is the same as the scale value on the transform.

## See Also

### Scaling an entity

func scale(relativeTo: Entity?) -> SIMD3&lt;Float>

Gets the scale of an entity relative to the given entity.

func setScale(SIMD3&lt;Float>, relativeTo: Entity?)

Sets the scale factor of the entity relative to the given reference entity.

