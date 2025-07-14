

- RealityKit
- Entity
-  convert(position:from:) 

Instance Method

# convert(position:from:)

Converts a position from the local space of a reference entity to the local space of the entity on which you called this method.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func convert(
    position: SIMD3,
    from referenceEntity: Entity?
) -> SIMD3
```

## Parameters 

`position`  

The position specified relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Return Value

The position given in the local space of the entity.

