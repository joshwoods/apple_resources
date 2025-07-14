

- RealityKit
-  PhysicsPrismaticJoint 

Structure

# PhysicsPrismaticJoint

A joint that allows movement along a straight line, similar to a sliding drawer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsPrismaticJoint
```

## Overview

`PhysicsPrismaticJoint`, also called a “slider joint”, allows one linear degree of freedom along the x-axis between two Entity pins.

Tip

Pass an orientation when creating the GeometricPin instances to change the axis of rotation.

## Topics

### Operators

static func == (PhysicsPrismaticJoint, PhysicsPrismaticJoint) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(pin0: GeometricPin, pin1: GeometricPin, linearLimit: ClosedRange&lt;Float>?, checksForInternalCollisions: Bool)

Creates a new prismatic joint.

### Instance Properties

var checksForInternalCollisions: Bool

A Boolean that indicates whether the joint checks and reports collisions between the two entity instances.

var isActive: Bool

A Boolean that indicates whether the joint is active.

var linearLimit: ClosedRange&lt;Float>?

A limit of the translation between the pins in the direction of the x-axis.

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

