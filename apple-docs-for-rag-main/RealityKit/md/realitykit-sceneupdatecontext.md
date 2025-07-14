

- RealityKit
-  SceneUpdateContext 

Structure

# SceneUpdateContext

An object that contains information about the scene to update.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct SceneUpdateContext
```

## Mentioned in 

Passing Metal command objects around your application

## Overview

RealityKit uses a SceneUpdateContext to pass information to a System about the scene it’s currently updating.

## Topics

### Updating a scene

var scene: Scene

The updating scene.

var deltaTime: TimeInterval

The number of seconds elapsed since the last update.

### Instance Methods

func entities(matching: EntityQuery, updatingSystemWhen: SystemUpdateCondition) -> QueryResult&lt;Entity>

Returns all entities which pass the query predicate of the query.

## See Also

### System configuration

Implementing systems for entities in a scene

Apply behaviors and physical effects to the objects and characters in a RealityKit scene with the Entity Component System (ECS).

protocol System

An object that affects multiple entities in every update of a RealityKit scene.

struct SystemUpdateCondition

A condition which causes a system to update.

