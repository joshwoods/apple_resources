

- RealityKit
- Entity
-  components 

Instance Property

# components

All the components that an entity stores.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var components: Entity.ComponentSet { get set }
```

## Discussion

You can only store one component of a given type on an entity.

## See Also

### Managing components

struct ComponentSet

A collection of components that an entity stores.

