

- RealityKit
- PhysicsCustomJoint
-  addToSimulation() 

Instance Method

# addToSimulation()

Adds this joint to the simulation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult @MainActor
func addToSimulation() throws -> Entity
```

## Return Value

The entity that owns the PhysicsJointsComponent, which this joint has been added to.

## Discussion

This method looks for an ancestral Entity that has PhysicsJointsComponent by traversing upwards from the entity referenced by pin0.

If found, it adds the joint to that ancestor’s PhysicsJointsComponent.

The traversal stops when reaching an Entity with PhysicsSimulationComponent, or when it cannot traverse up anymore. In the former case it adds the joint to joints. In the latter case it adds PhysicsJointsComponent to the first Entity referenced by the joint, and adds the joint to the newly created PhysicsJointsComponent.

Throws

When the joint contains invalid data.

