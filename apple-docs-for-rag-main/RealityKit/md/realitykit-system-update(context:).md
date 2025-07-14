

- RealityKit
- System
-  update(context:) 

Instance Method

# update(context:)

Updates entities up to once every scene update.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
mutating func update(context: SceneUpdateContext)
```

**Required** Default implementation provided.

## Parameters 

`context`  

The scene context for the scene to update.

## Mentioned in 

Implementing systems for entities in a scene

## Discussion

RealityKit calls this method on all registered systems, as often as the `updatingSystemWhen` parameter of entities(matching:updatingSystemWhen:) defines.

The `context` parameter contains a reference to the scene that the System is updating, along with the elapsed time since RealityKit last called the update method for the same scene. Use entities(matching:updatingSystemWhen:) inside this method for the most optimized way to find the matching entities for this System.

## Default Implementations

### System Implementations

func update(context: SceneUpdateContext)

A default implementation that does nothing.

## See Also

### Implementing system logic

struct SceneUpdateContext

An object that contains information about the scene to update.

struct EntityQuery

An object that retrieves entities from a scene.

struct QueryPredicate

An object that defines the criteria for an entity query.

struct QueryResult

An object that returns the results of an entity query.

