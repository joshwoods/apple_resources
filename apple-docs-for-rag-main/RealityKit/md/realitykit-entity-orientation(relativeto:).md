

- RealityKit
- Entity
-  orientation(relativeTo:) 

Instance Method

# orientation(relativeTo:)

Gets the orientation of an entity relative to the given entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func orientation(relativeTo referenceEntity: Entity?) -> simd_quatf
```

## Parameters 

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Return Value

The orientation of the entity relative to `referenceEntity`.

