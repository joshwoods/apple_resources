

- RealityKit
- Entity
-  init(components:) 

Initializer

# init(components:)

Creates an entity with one or multiple components.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor @preconcurrency
convenience init(components: repeat each T) where repeat each T : Component
```

## Parameters 

`components`  

A comma-delimited list of components to add to the entity.

## Discussion

The components you specify in this initializer override any default components of the same type that RealityKit creates the entity with, such as Transform.

For example, you can use this initializer to create an entity that has a SpotLightComponent:

```
let spotlightEntity = Entity(components: SpotLightComponent())
```

You can also create an entity with multiple initial components, such as a ModelComponent and a Transform:

```
let sphereEntity = Entity(
    components: ModelComponent(mesh: .generateBox(size: 1), materials: []),
                Transform(translation: [0, 0.5, 0])
)
```

Note

You can change any of the entity’s components at any time by modifying the entity’s components set.

## See Also

### Creating an entity

init()

Creates a new entity.

convenience init(components: [any Component])

Creates an entity with multiple components.

func clone(recursive: Bool) -> Self

Duplicates an entity to create a new entity.

func didClone(from: Entity)

Tells a newly cloned entity that cloning is complete.

