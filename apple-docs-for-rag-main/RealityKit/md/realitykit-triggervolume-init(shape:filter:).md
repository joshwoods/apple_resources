

- RealityKit
- TriggerVolume
-  init(shape:filter:) 

Initializer

# init(shape:filter:)

Creates a trigger volume with the given shape and collision filter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
convenience init(
    shape: ShapeResource,
    filter: CollisionFilter = .sensor
)
```

## Parameters 

`shape`  

The shape of the trigger volume.

`filter`  

A collision filter that lets you differentiate among collision groups.

## See Also

### Creating a trigger volume

init()

Creates a trigger volume.

init(shapes: [ShapeResource], filter: CollisionFilter)

Creates a trigger volume with the given composite shape and collision filter.

