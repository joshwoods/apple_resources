

- RealityKit
- Entity
-  convert(direction:from:) 

Instance Method

# convert(direction:from:)

Converts a direction vector from the local space of a reference entity to the local space of the entity on which you called this method.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func convert(
    direction: SIMD3,
    from referenceEntity: Entity?
) -> SIMD3
```

## Parameters 

`direction`  

The direction vector specified relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Return Value

The direction vector given in the local space of the entity.

