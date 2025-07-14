

- RealityKit
- PhysicsSphericalJoint
-  isActive 

Instance Property

# isActive

A Boolean that indicates whether the joint is active.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var isActive: Bool { get }
```

## Discussion

Inactive joints do not participate in the physics simulation.

One example is a joint that does not reference any Entity with PhysicsBodyMode.dynamic, or when one or both the referenced entities are not active.

