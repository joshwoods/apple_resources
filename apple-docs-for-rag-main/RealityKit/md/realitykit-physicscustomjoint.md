

- RealityKit
-  PhysicsCustomJoint 

Structure

# PhysicsCustomJoint

A joint with six degrees of freedom that can be individually specified.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsCustomJoint
```

## Overview

A custom joint allows you to choose the restraints of all 6 degrees of freedom. You can set a PhysicsCustomJoint.MotionLimit for each degrees’ motion.

Note

By default all degrees of freedom are locked, similar to PhysicsFixedJoint.

For example, you can constrain the motion of pin1 in the xy-plane of pin0, set movement along the x-axis to PhysicsCustomJoint.MotionLimit.unlimited, and leave all rotations as the default value of PhysicsCustomJoint.MotionLimit.fixed.

Note

The xy-plane is a plane that aligns with the x and y axes.

```
let joint = PhysicsCustomJoint(
    pin0: entity0pin,
    pin1: entity1pin,
    linearMotionAlongX: .unlimited,
    linearMotionAlongY: .range(-5...5)
)
```

If pin0 is in a fixed location for the example above, this joint allows pin1 to move anywhere along the x-axis of pin0, and can move up to 5 local meters above or below the y-axis of pin0.

## Topics

### Operators

static func == (PhysicsCustomJoint, PhysicsCustomJoint) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(pin0: GeometricPin, pin1: GeometricPin, linearMotionAlongX: PhysicsCustomJoint.MotionLimit, linearMotionAlongY: PhysicsCustomJoint.MotionLimit, linearMotionAlongZ: PhysicsCustomJoint.MotionLimit, angularMotionAroundX: PhysicsCustomJoint.MotionLimit, angularMotionAroundY: PhysicsCustomJoint.MotionLimit, angularMotionAroundZ: PhysicsCustomJoint.MotionLimit, checksForInternalCollisions: Bool)

Creates a new custom joint.

### Instance Properties

var angularMotionAroundX: PhysicsCustomJoint.MotionLimit

The angular motion limits around the x-axis.

var angularMotionAroundY: PhysicsCustomJoint.MotionLimit

The angular motion limits around the y-axis.

var angularMotionAroundZ: PhysicsCustomJoint.MotionLimit

The angular motion limits around the z-axis.

var checksForInternalCollisions: Bool

A Boolean that indicates whether the joint checks and reports collisions between the two entity instances.

var isActive: Bool

A Boolean that indicates whether the joint is active.

var linearMotionAlongX: PhysicsCustomJoint.MotionLimit

The linear motion limits along the x-axis.

var linearMotionAlongY: PhysicsCustomJoint.MotionLimit

The linear motion limits along the y-axis.

var linearMotionAlongZ: PhysicsCustomJoint.MotionLimit

The linear motion limits along the z-axis.

var pin0: GeometricPin

The pin that defines a local position and orientation on the first entity.

var pin1: GeometricPin

The pin that defines a local position and orientation on the second entity.

### Enumerations

enum MotionLimit

Specifies allowed linear or angular motion.

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

struct PhysicsSphericalJoint

A spherical joint that allows free rotational movement between two entities’ pins.

struct PhysicsDistanceJoint

A joint that maintains a minimum and maximum distance between two entity pins.

struct PhysicsFixedJoint

A joint that rigidly connects two entity pins, with zero degrees of freedom.

struct PhysicsJoints

A collection of physics joints.

