

- RealityKit
- Entity
-  convert(transform:from:) 

Instance Method

# convert(transform:from:)

Converts the scale, rotation, and position of a transform from the local space of a reference entity to the local space of the entity on which you called this method.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func convert(
    transform: Transform,
    from referenceEntity: Entity?
) -> Transform
```

## Parameters 

`transform`  

The transform specified relative to `referenceEntity`.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Return Value

The transform given in the local space of the entity.

