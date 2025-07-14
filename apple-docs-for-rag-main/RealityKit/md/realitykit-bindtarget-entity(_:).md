

- RealityKit
- BindTarget
-  entity(\_:) 

Type Method

# entity(\_:)

Generates a complex bind path from a particular child entity of the current entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static func entity(_ name: String) -> BindTarget.EntityPath
```

## See Also

### Targeting entities and scenes

static func scene(String) -> BindTarget.ScenePath

Generates a bind path from a particular scene.

struct ScenePath

A bind path for a particular scene.

static func anchorEntity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular anchor entity in the scene.

struct EntityPath

A bind path context for a particular entity.

