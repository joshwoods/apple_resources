

- RealityKit
- PhysicsJoint
-  checksForInternalCollisions 

Instance Property

# checksForInternalCollisions

A Boolean that indicates whether the joint checks and reports collisions between the two entity instances.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var checksForInternalCollisions: Bool { get }
```

**Required**

## Discussion

Note

This does not affect how collisions of the two entities referenced in pin0 and pin1 interact with other entities.

