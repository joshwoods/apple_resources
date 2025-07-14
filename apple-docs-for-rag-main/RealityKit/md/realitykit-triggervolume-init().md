

- RealityKit
- TriggerVolume
-  init() 

Initializer

# init()

Creates a trigger volume.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
required init()
```

## See Also

### Creating a trigger volume

convenience init(shape: ShapeResource, filter: CollisionFilter)

Creates a trigger volume with the given shape and collision filter.

init(shapes: [ShapeResource], filter: CollisionFilter)

Creates a trigger volume with the given composite shape and collision filter.

