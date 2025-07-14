

- RealityKit
- Entity
-  init() 

Initializer

# init()

Creates a new entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
required init()
```

## See Also

### Creating an entity

convenience init&lt;each T>(components: repeat each T)

Creates an entity with one or multiple components.

convenience init(components: [any Component])

Creates an entity with multiple components.

func clone(recursive: Bool) -> Self

Duplicates an entity to create a new entity.

func didClone(from: Entity)

Tells a newly cloned entity that cloning is complete.

