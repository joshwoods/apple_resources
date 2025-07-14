

- RealityKit
- AnchoringComponent
-  init(\_:trackingMode:physicsSimulation:) 

Initializer

# init(\_:trackingMode:physicsSimulation:)

Creates an anchoring component for a given target, tracking mode and physics simulation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    _ target: AnchoringComponent.Target,
    trackingMode: AnchoringComponent.TrackingMode,
    physicsSimulation: AnchoringComponent.PhysicsSimulation = .isolated
)
```

## Parameters 

`target`  

The kind of real world object to target.

`trackingMode`  

The tracking mode of the entity.

`physicsSimulation`  

The physics simulation space the entity will be in.

## See Also

### Creating the anchor component

init(AnchoringComponent.Target)

Creates an anchoring component for a given target.

init(AnchoringComponent.Target, trackingMode: AnchoringComponent.TrackingMode)

init(ARAnchor)

Creates an anchoring component with the given AR anchor.

