

- RealityKit
- Entity
-  findEntity(named:) 

Instance Method

# findEntity(named:)

Recursively searches all descendant entities for one with the given name.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func findEntity(named name: String) -> Entity?
```

## Parameters 

`name`  

The entity name for which to search.

## Return Value

An entity with the given name, or `nil` if no entity is found.

## Discussion

The findEntity(named:) method conducts a depth-first, recursive search over all of the entity’s descendants for one whose name property matches the given name. The method returns the first match. Entity names need not be unique.

## See Also

### Inspecting an entity

var scene: Scene?

The scene that owns the entity.

var name: String

The name of the entity.

var id: UInt64

The stable identity of the entity associated with this instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

var debugDescription: String

A human readable description of the entity.

