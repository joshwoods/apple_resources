

- RealityKit
- BindTarget
-  scene(\_:) 

Type Method

# scene(\_:)

Generates a bind path from a particular scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static func scene(_ name: String) -> BindTarget.ScenePath
```

## See Also

### Targeting entities and scenes

struct ScenePath

A bind path for a particular scene.

static func anchorEntity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular anchor entity in the scene.

static func entity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular child entity of the current entity.

struct EntityPath

A bind path context for a particular entity.

