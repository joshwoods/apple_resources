

- RealityKit
- Entity
-  scene 

Instance Property

# scene

The scene that owns the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var scene: Scene? { get }
```

## Discussion

An entity belongs to a scene if the entity is part of a hierarchy that’s rooted in the scene’s anchors collection.

The value of the property is `nil` if the entity isn’t currently attached to any scene.

## See Also

### Inspecting an entity

var name: String

The name of the entity.

func findEntity(named: String) -> Entity?

Recursively searches all descendant entities for one with the given name.

var id: UInt64

The stable identity of the entity associated with this instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

var debugDescription: String

A human readable description of the entity.

