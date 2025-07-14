

- RealityKit
- PhysicsSphericalJoint
-  init(pin0:pin1:angularLimitInYZ:checksForInternalCollisions:) 

Initializer

# init(pin0:pin1:angularLimitInYZ:checksForInternalCollisions:)

Creates a new spherical joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    pin0: GeometricPin,
    pin1: GeometricPin,
    angularLimitInYZ: (Float, Float)? = nil,
    checksForInternalCollisions: Bool = false
)
```

## Parameters 

`pin0`  

The local position and orientation on the first entity.

`pin1`  

The local position and orientation on the second entity.

`angularLimitInYZ`  

A maximum value of rotation in radians from the y and z axes if defined.

`checksForInternalCollisions`  

A Boolean that indicates whether the joint checks for collisions between the two Entity instances.

## Discussion

An elliptical cone is formed around the x-axis to limit the motion of `pin1` if `angularLimitInYZ` is defined.

If `angularLimitInYZ` is undefined, `pin1` has full 360º rotational freedom in all axes.

