

- RealityKit
- PhysicsSimulationComponent
- PhysicsSimulationComponent.SolverIterations
-  init(positionIterations:velocityIterations:) 

Initializer

# init(positionIterations:velocityIterations:)

Creates a solver iterations configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    positionIterations: Int = 6,
    velocityIterations: Int = 1
)
```

## Parameters 

`positionIterations`  

The number of position iterations the solver performs, in the inclusive range `[1, 255]`. The default value is `6`.

`velocityIterations`  

The number of velocity iterations the solver performs, in the inclusive range `[1, 255]`. The default value is `1`.

