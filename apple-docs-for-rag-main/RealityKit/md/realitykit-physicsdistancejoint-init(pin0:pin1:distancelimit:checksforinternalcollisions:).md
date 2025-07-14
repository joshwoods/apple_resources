

- RealityKit
- PhysicsDistanceJoint
-  init(pin0:pin1:distanceLimit:checksForInternalCollisions:) 

Initializer

# init(pin0:pin1:distanceLimit:checksForInternalCollisions:)

Creates a new distance joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    pin0: GeometricPin,
    pin1: GeometricPin,
    distanceLimit: ClosedRange,
    checksForInternalCollisions: Bool = false
)
```

## Parameters 

`pin0`  

The local position and orientation on the first entity.

`pin1`  

The local position and orientation on the second entity.

`distanceLimit`  

Specifies the minimum and maximum allowed distance between the two pins.

`checksForInternalCollisions`  

A Boolean that indicates whether the joint checks for collisions between the two Entity instances.

