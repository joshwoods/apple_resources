

- RealityKit
-  SystemUpdateCondition 

Structure

# SystemUpdateCondition

A condition which causes a system to update.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct SystemUpdateCondition
```

## Topics

### Type Properties

static var rendering: SystemUpdateCondition

A condition that is active whenever an update for rendering may be needed, usually matching the refresh rate of the display.

## See Also

### System configuration

Implementing systems for entities in a scene

Apply behaviors and physical effects to the objects and characters in a RealityKit scene with the Entity Component System (ECS).

protocol System

An object that affects multiple entities in every update of a RealityKit scene.

struct SceneUpdateContext

An object that contains information about the scene to update.

