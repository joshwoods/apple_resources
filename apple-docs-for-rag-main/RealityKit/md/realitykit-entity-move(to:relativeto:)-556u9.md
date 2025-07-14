

- RealityKit
- Entity
-  move(to:relativeTo:) 

Instance Method

# move(to:relativeTo:)

Moves an entity instantly to a new location given by a transform.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func move(
    to transform: Transform,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`transform`  

A Transform instance that indicates the new location.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

