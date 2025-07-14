

- RealityKit
- PhysicsRevoluteJoint
-  init(pin0:pin1:angularLimit:checksForInternalCollisions:) 

Initializer

# init(pin0:pin1:angularLimit:checksForInternalCollisions:)

Creates a new revolute joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    pin0: GeometricPin,
    pin1: GeometricPin,
    angularLimit: ClosedRange? = nil,
    checksForInternalCollisions: Bool = false
)
```

## Parameters 

`pin0`  

The local position and orientation on the first entity.

`pin1`  

The local position and orientation on the second entity.

`angularLimit`  

Limits of the rotation around the pin’s x-axis if defined.

`checksForInternalCollisions`  

A Boolean that indicates whether the joint checks for collisions between the two Entity instances.

