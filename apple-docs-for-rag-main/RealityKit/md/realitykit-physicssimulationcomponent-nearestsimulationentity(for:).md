

- RealityKit
- PhysicsSimulationComponent
-  nearestSimulationEntity(for:) 

Type Method

# nearestSimulationEntity(for:)

Obtains the entity containing the physics simulation origin.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static func nearestSimulationEntity(for entity: Entity) -> Entity?
```

## Parameters 

`entity`  

The entity to find the physics simulation origin for.

## Return Value

The entity containing the physics simulation origin or `nil` if the entity doesn’t have a parent object in the scene.

## Discussion

The simulation origin is the nearest parent object where a PhysicsSimulationComponent exists, or the root entity (normally the anchor) where the default simulation is embedded.

