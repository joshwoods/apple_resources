

- RealityKit
- PhysicsSimulationComponent
-  gravity 

Instance Property

# gravity

The gravity for the simulation relative to the simulation entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var gravity: SIMD3
```

## Discussion

The value stored in this property is the gravitational acceleration applied to dynamic physics body entities every frame along the negative world y-axis. The default value is `-9.81` meters per second squared.

