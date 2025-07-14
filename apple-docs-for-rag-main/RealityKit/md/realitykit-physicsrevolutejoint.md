

- RealityKit
-  PhysicsRevoluteJoint 

Structure

# PhysicsRevoluteJoint

A joint that allows one degree of rotational freedom between two entity pins, similar to a door swinging on its hinges.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsRevoluteJoint
```

## Overview

`PhysicsRevoluteJoint` allows one rotational degree of freedom along the x-axis of two entity pins.

Tip

Pass an orientation when creating the GeometricPin instances to change the axis of rotation.

## Topics

### Operators

static func == (PhysicsRevoluteJoint, PhysicsRevoluteJoint) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(pin0: GeometricPin, pin1: GeometricPin, angularLimit: ClosedRange&lt;Float>?, checksForInternalCollisions: Bool)

Creates a new revolute joint.

### Instance Properties

var angularLimit: ClosedRange&lt;Float>?

A limit of the rotational freedom between the pins around the x-axis.

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

struct PhysicsPrismaticJoint

A joint that allows movement along a straight line, similar to a sliding drawer.

struct PhysicsSphericalJoint

A spherical joint that allows free rotational movement between two entities’ pins.

struct PhysicsCustomJoint

A joint with six degrees of freedom that can be individually specified.

struct PhysicsDistanceJoint

A joint that maintains a minimum and maximum distance between two entity pins.

struct PhysicsFixedJoint

A joint that rigidly connects two entity pins, with zero degrees of freedom.

struct PhysicsJoints

A collection of physics joints.

