

- RealityKit
- Entity
-  setOrientation(\_:relativeTo:) 

Instance Method

# setOrientation(\_:relativeTo:)

Sets the orientation of the entity relative to the given reference entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func setOrientation(
    _ orientation: simd_quatf,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`orientation`  

A new orientation, relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

