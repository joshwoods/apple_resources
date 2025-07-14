

- RealityKit
-  System 

Protocol

# System

An object that affects multiple entities in every update of a RealityKit scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol System
```

## Mentioned in 

Implementing systems for entities in a scene

Passing Metal command objects around your application

## Overview

In RealityKit’s Entity Component System (ECS), a *system* represents continuous behavior that affects multiple entities in the scene. Use systems to implement any behavior or logic that updates entities every scene update, such as different types of objects or characters. For example, a physics simulation system calculates and applies the affect of gravity, forces, and collisions for all entities. A system calls the update(context:) method as often as the `updatingSystemWhen` parameter of entities(matching:updatingSystemWhen:) defines.

Systems often work with components. You might, for example, create a system that calculates the hunger levels for entities in a game capable of feeling hunger. To identify which entities experience hunger, use a component that stores hunger-related state data and add it to the selected entities. The hunger system then iterates through all entities that contain a hunger component and updates their state based on relevant factors, such as when the entity last ate or how much energy it expends.

A complex game or experience may consist of many systems which need to be executed in a specific order. The dependencies property defines when the `update` method for each system is called each frame. Update order is defined between system types and not between individual system instances.

Systems and their dependencies form a directed acyclic graph (DAG). Custom systems are executed in dependency order. Systems without dependencies are updated in the order they were registered. If there are conflicting dependencies or cycles, then RealityKit ignores some conflicting dependencies and logs a warning. Each system instance is only run once per simulation step.

Properties of a system are never serialized to a file or synced over the network. Therefore, store data on entities using components, rather than as part of the system.

For more information, see Implementing systems for entities in a scene.

## Topics

### Registering a system

static func registerSystem()

Registers a system with RealityKit.

### Specifying dependencies

static var dependencies: [SystemDependency]

An array of dependencies for this system.

**Required** Default implementation provided.

enum SystemDependency

Defines update order relative to other systems. An object that specifies the update order between multiple systems.

### Creating a system

init(scene: Scene)

Creates a new system.

**Required**

### Implementing system logic

func update(context: SceneUpdateContext)

Updates entities up to once every scene update.

**Required** Default implementation provided.

struct SceneUpdateContext

An object that contains information about the scene to update.

struct EntityQuery

An object that retrieves entities from a scene.

struct QueryPredicate

An object that defines the criteria for an entity query.

struct QueryResult

An object that returns the results of an entity query.

## See Also

### System configuration

Implementing systems for entities in a scene

Apply behaviors and physical effects to the objects and characters in a RealityKit scene with the Entity Component System (ECS).

struct SystemUpdateCondition

A condition which causes a system to update.

struct SceneUpdateContext

An object that contains information about the scene to update.

