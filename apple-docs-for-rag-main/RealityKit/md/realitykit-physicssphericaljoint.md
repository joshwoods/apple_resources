

- RealityKit
-  PhysicsSphericalJoint 

Structure

# PhysicsSphericalJoint

A spherical joint that allows free rotational movement between two entities’ pins.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsSphericalJoint
```

## Overview

This joint has three rotational degrees of freedom and removes all translational degrees of freedom by making the positions of pin0 and pin1 coincide. This is also called a “ball-socket joint”.

To add limits to the rotational freedom of pin1, define a tuple value for angularLimitInYZ. This tuple defines an elliptical cone shape around the x-axis of pin0, which limits the rotational freedom of pin1. The rotation around the x-axis is never limited with this joint.

Tip

Pass an orientation when creating the GeometricPin instances to change the axis of rotation.

## Topics

### Operators

static func == (PhysicsSphericalJoint, PhysicsSphericalJoint) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(pin0: GeometricPin, pin1: GeometricPin, angularLimitInYZ: (Float, Float)?, checksForInternalCollisions: Bool)

Creates a new spherical joint.

### Instance Properties

var angularLimitInYZ: (Float, Float)?

A cone-shaped limit of rotational freedom.

var checksForInternalCollisions: Bool

A Boolean that indicates whether the joint checks and reports collisions between the two entity instances.

var isActive: Bool

A Boolean that indicates whether the joint is active.

var pin0: GeometricPin

The pin that defines a local position and orientation on the first entity.

var pin1: GeometricPin

The pin that defines a local position and orientation on the second entity.

### Default Implementations

Equatable Implementations

PhysicsJoint Implementations

## Relationships

### Conforms To

- Equatable
- PhysicsJoint

## See Also

### Built-in joint types

struct PhysicsRevoluteJoint

A joint that allows one degree of rotational freedom between two entity pins, similar to a door swinging on its hinges.

struct PhysicsPrismaticJoint

A joint that allows movement along a straight line, similar to a sliding drawer.

struct PhysicsCustomJoint

A joint with six degrees of freedom that can be individually specified.

struct PhysicsDistanceJoint

A joint that maintains a minimum and maximum distance between two entity pins.

struct PhysicsFixedJoint

A joint that rigidly connects two entity pins, with zero degrees of freedom.

struct PhysicsJoints

A collection of physics joints.

