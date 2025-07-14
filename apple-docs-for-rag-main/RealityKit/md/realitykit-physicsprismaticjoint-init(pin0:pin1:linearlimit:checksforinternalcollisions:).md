

- RealityKit
- PhysicsPrismaticJoint
-  init(pin0:pin1:linearLimit:checksForInternalCollisions:) 

Initializer

# init(pin0:pin1:linearLimit:checksForInternalCollisions:)

Creates a new prismatic joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    pin0: GeometricPin,
    pin1: GeometricPin,
    linearLimit: ClosedRange? = nil,
    checksForInternalCollisions: Bool = false
)
```

## Parameters 

`pin0`  

The local position and orientation on the first entity.

`pin1`  

The local position and orientation on the second entity.

`linearLimit`  

A limit of the the translation of `pin1` from `pin0` in the direction of the x-axis of `pin0`.

`checksForInternalCollisions`  

A Boolean that indicates whether the joint checks for collisions between the two Entity instances.

