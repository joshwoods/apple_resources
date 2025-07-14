

- RealityKit
- Entity
- Entity.ComponentSet
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the component of the specified type from the collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func remove(_ componentType: any Component.Type)
```

## See Also

### Updating the set

func set&lt;T>(T)

Adds a new component to the set, or overrides an existing one.

func set([any Component])

Adds multiple components to the set, overriding any existing components of the same type.

func removeAll()

Removes all components from the collection.

