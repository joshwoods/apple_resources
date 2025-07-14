

- RealityKit
- Entity
-  position(relativeTo:) 

Instance Method

# position(relativeTo:)

Gets the position of an entity relative to the given entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func position(relativeTo referenceEntity: Entity?) -> SIMD3
```

## Parameters 

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Return Value

The position of the entity relative to `referenceEntity`.

