

- RealityKit
- IKRig
- IKRig.Constraint
- IKRig.Constraint.IKPositionDemand
-  weight 

Instance Property

# weight

The per-axis weight this demand has on the pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var weight: SIMD3
```

## Discussion

Note

Values of `0` or less remove the demand influence.

