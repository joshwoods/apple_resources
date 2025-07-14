

- RealityKit
- Entity
-  didClone(from:) 

Instance Method

# didClone(from:)

Tells a newly cloned entity that cloning is complete.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func didClone(from source: Entity)
```

## Parameters 

`source`  

The entity from which the cloned entity was copied.

## Discussion

This method clones all component data automatically. When you clone an entity that stores custom data that’s not part of a component, override the didClone(from:) method to copy that data manually after the clone finishes.

## See Also

### Creating an entity

init()

Creates a new entity.

convenience init&lt;each T>(components: repeat each T)

Creates an entity with one or multiple components.

convenience init(components: [any Component])

Creates an entity with multiple components.

func clone(recursive: Bool) -> Self

Duplicates an entity to create a new entity.

