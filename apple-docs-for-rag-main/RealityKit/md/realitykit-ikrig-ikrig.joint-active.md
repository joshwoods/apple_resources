

- RealityKit
- IKRig
- IKRig.Joint
-  active 

Instance Property

# active

A boolean value that sets whether the solver rotates the joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var active: Bool
```

## Discussion

Leaf hierarchies that do not need to be directly constrained can be deactivated to reduce the compute cost of the solver.

