

- RealityKit
- IKRig
- IKRig.Constraint
- IKRig.Constraint.IKPositionDemand
-  influenceDepthMaxJointCount 

Instance Property

# influenceDepthMaxJointCount

The number of joints to be influenced by this demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var influenceDepthMaxJointCount: Int
```

## Discussion

The count starts from the constrained joint and continues up the chain to the skeleton’s root.

Note

A depth of `0` disables the constraint, while negative values are treated as `Int.max`

