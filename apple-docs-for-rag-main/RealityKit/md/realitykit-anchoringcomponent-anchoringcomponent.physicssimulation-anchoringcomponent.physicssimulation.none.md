

- RealityKit
- AnchoringComponent
- AnchoringComponent.PhysicsSimulation
-  AnchoringComponent.PhysicsSimulation.none 

Case

# AnchoringComponent.PhysicsSimulation.none

Opts out the entity and its descendants from having their own physics space.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case none
```

## Discussion

`none` implies the anchor entity does not have its own physics simulation.

It will use the regular rules to determine which physics simulation the entity is a part of. For more about the rules, please check PhysicsSimulationComponent.

