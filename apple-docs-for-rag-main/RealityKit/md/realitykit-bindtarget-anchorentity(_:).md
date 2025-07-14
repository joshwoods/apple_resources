

- RealityKit
- BindTarget
-  anchorEntity(\_:) 

Type Method

# anchorEntity(\_:)

Generates a complex bind path from a particular anchor entity in the scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static func anchorEntity(_ name: String) -> BindTarget.EntityPath
```

## See Also

### Targeting entities and scenes

static func scene(String) -> BindTarget.ScenePath

Generates a bind path from a particular scene.

struct ScenePath

A bind path for a particular scene.

static func entity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular child entity of the current entity.

struct EntityPath

A bind path context for a particular entity.

