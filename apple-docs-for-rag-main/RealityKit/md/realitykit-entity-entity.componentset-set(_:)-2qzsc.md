

- RealityKit
- Entity
- Entity.ComponentSet
-  set(\_:) 

Instance Method

# set(\_:)

Adds multiple components to the set, overriding any existing components of the same type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func set(_ components: [any Component])
```

## Parameters 

`components`  

An array of components to add.

## Discussion

If the input array includes multiple components of the same type, the set adds the component with the highest index. This is because the set can only hold one component of each type.

## See Also

### Updating the set

func set&lt;T>(T)

Adds a new component to the set, or overrides an existing one.

func remove(any Component.Type)

Removes the component of the specified type from the collection.

func removeAll()

Removes all components from the collection.

