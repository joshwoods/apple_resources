

- RealityKit
- Entity
-  Entity.ComponentSet 

Structure

# Entity.ComponentSet

A collection of components that an entity stores.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
struct ComponentSet
```

## Overview

A `ComponentSet` represents all the components that an entity holds. Use this set to add, remove, and update components on an entity. This set can hold one component of each type.

Access the `ComponentSet` of an Entity using its components property.

`ComponentSet` conforms to Sequence, allowing you to iterate over it to access and use each component, as the example below shows:

```
for component in entity.components {
    print(component)
}
```

## Topics

### Updating the set

func set&lt;T>(T)

Adds a new component to the set, or overrides an existing one.

func set([any Component])

Adds multiple components to the set, overriding any existing components of the same type.

func remove(any Component.Type)

Removes the component of the specified type from the collection.

func removeAll()

Removes all components from the collection.

### Accessing members

subscript&lt;T>(T.Type) -> T?

Gets or sets the component of the specified type.

subscript(any Component.Type) -> (any Component)?

Gets or sets the component with a specific dynamically supplied type.

### Counting members

var count: Int

The number of components in the collection.

### Checking for membership

func has(any Component.Type) -> Bool

Returns a Boolean value that indicates whether the set contains a component of the given type.

### Default Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- Sendable
- Sequence

## See Also

### Managing components

var components: Entity.ComponentSet

All the components that an entity stores.

