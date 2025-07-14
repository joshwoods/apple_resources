

- RealityKit
- RadialForceEffect
-  restDistance 

Instance Property

# restDistance

A distance at which the rigid bodies receive zero radial force.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let restDistance: Float
```

## Discussion

Use a **non-negative** rate. The force field pulls rigid bodies to the effect’s origin along the radial direction if this value is `0`.

