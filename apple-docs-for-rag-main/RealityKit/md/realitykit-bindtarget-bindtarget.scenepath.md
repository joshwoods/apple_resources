

- RealityKit
- BindTarget
-  BindTarget.ScenePath 

Structure

# BindTarget.ScenePath

A bind path for a particular scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct ScenePath
```

## Overview

This structure defines an absolute bind path for a scene. You determine the scene that a particular instance references by specifying the scene’s name as the argument to BindPath.Part.scene(_:).

## Topics

### Accessing the anchor entity

func anchorEntity(String) -> BindTarget.EntityPath

A path for the scene’s anchor entity.

### Accessing the bind target

var `self`: BindTarget

A bind target for the scene.

## See Also

### Targeting entities and scenes

static func scene(String) -> BindTarget.ScenePath

Generates a bind path from a particular scene.

static func anchorEntity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular anchor entity in the scene.

static func entity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular child entity of the current entity.

struct EntityPath

A bind path context for a particular entity.

