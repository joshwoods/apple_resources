

- RealityKit
- HasTransform
-  setScale(\_:relativeTo:) 

Instance Method

# setScale(\_:relativeTo:)

Sets the scale factor of the entity relative to the given reference entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func setScale(
    _ scale: SIMD3,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`scale`  

A new scale factor, relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## See Also

### Scaling an entity

var scale: SIMD3&lt;Float>

The scale of the entity relative to its parent.

func scale(relativeTo: Entity?) -> SIMD3&lt;Float>

Gets the scale of an entity relative to the given entity.

