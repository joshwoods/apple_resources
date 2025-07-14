

- RealityKit
- PhysicsFixedJoint
-  checksForInternalCollisions 

Instance Property

# checksForInternalCollisions

A Boolean that indicates whether the joint checks and reports collisions between the two entity instances.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let checksForInternalCollisions: Bool
```

## Discussion

The entities that PhysicsFixedJoint references are not checked or reported, so this property only returns `false`.

