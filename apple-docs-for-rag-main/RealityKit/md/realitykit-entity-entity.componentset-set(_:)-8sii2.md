

- RealityKit
- Entity
- Entity.ComponentSet
-  set(\_:) 

Instance Method

# set(\_:)

Adds a new component to the set, or overrides an existing one.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func set(_ component: T) where T : Component
```

## Parameters 

`component`  

The component to add.

## See Also

### Updating the set

func set([any Component])

Adds multiple components to the set, overriding any existing components of the same type.

func remove(any Component.Type)

Removes the component of the specified type from the collection.

func removeAll()

Removes all components from the collection.

