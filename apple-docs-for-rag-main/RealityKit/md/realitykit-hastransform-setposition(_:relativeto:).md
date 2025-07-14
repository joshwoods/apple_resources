

- RealityKit
- HasTransform
-  setPosition(\_:relativeTo:) 

Instance Method

# setPosition(\_:relativeTo:)

Sets the position of the entity relative to the given reference entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func setPosition(
    _ position: SIMD3,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`position`  

A new position, relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## See Also

### Positioning an entity

var position: SIMD3&lt;Float>

The position of the entity relative to its parent.

func position(relativeTo: Entity?) -> SIMD3&lt;Float>

Gets the position of an entity relative to the given entity.

