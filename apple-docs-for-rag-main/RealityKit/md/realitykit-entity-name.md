

- RealityKit
- Entity
-  name 

Instance Property

# name

The name of the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var name: String { get set }
```

## Discussion

You can find an entity by name in a scene by calling the scene’s findEntity(named:) method. Or you can recursively search among the children of a given entity by calling the entity’s findEntity(named:) method.

Entity names are not guaranteed to be unique. When you search by name, these methods return the first entity encountered with the given name.

## See Also

### Inspecting an entity

var scene: Scene?

The scene that owns the entity.

func findEntity(named: String) -> Entity?

Recursively searches all descendant entities for one with the given name.

var id: UInt64

The stable identity of the entity associated with this instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

var debugDescription: String

A human readable description of the entity.

