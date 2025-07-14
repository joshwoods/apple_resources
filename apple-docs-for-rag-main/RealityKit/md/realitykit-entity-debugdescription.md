

- RealityKit
- Entity
-  debugDescription 

Instance Property

# debugDescription

A human readable description of the entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var debugDescription: String { get }
```

## See Also

### Inspecting an entity

var scene: Scene?

The scene that owns the entity.

var name: String

The name of the entity.

func findEntity(named: String) -> Entity?

Recursively searches all descendant entities for one with the given name.

var id: UInt64

The stable identity of the entity associated with this instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

