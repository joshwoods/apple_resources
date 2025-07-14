

- RealityKit
- Entity
-  init(components:) 

Initializer

# init(components:)

Creates an entity with multiple components.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(components: [any Component])
```

## Parameters 

`components`  

The components to add to the entity.

## Discussion

This initializer adds the contents of `components` to the new Entity. The components you specify in this initializer override any default components of the same type that RealityKit creates the entity with, such as Transform.

For example, you can use this initializer to create an entity that anchors to the floor, displays a 1x1x1m box, and has a y-position of 0.5:

```
let floorCubeComponents = [
    AnchoringComponent(.plane(.horizontal, classification: .floor, minimumBounds: [1, 1])),
    ModelComponent(mesh: .generateBox(size: 1), materials: []),
    Transform(translation: [0, 0.5, 0])
]

let floorCubeEntity = Entity(components: floorCubeComponents)
```

Note

You can change any of the entity’s components at any time by modifying the entity’s components set.

## See Also

### Creating an entity

init()

Creates a new entity.

convenience init&lt;each T>(components: repeat each T)

Creates an entity with one or multiple components.

func clone(recursive: Bool) -> Self

Duplicates an entity to create a new entity.

func didClone(from: Entity)

Tells a newly cloned entity that cloning is complete.

