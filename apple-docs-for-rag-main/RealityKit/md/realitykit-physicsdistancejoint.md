

- RealityKit
-  PhysicsDistanceJoint 

Structure

# PhysicsDistanceJoint

A joint that maintains a minimum and maximum distance between two entity pins.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PhysicsDistanceJoint
```

## Overview

A distance joint restricts the distance between pin0 and pin1. The joint determines this closed range according to distanceLimit.

This joint allows full rotational freedom between pin0 and pin1.

## Topics

### Operators

static func == (PhysicsDistanceJoint, PhysicsDistanceJoint) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(pin0: GeometricPin, pin1: GeometricPin, distanceLimit: ClosedRange&lt;Float>, checksForInternalCollisions: Bool)

Creates a new distance joint.

### Instance Properties

var checksForInternalCollisions: Bool

A Boolean that indicates whether the joint checks and reports collisions between the two entity instances.

var distanceLimit: ClosedRange&lt;Float>

Specifies the minimum and maximum allowed distance between the pins.

var isActive: Bool

A Boolean that indicates whether the joint is active.

var pin0: GeometricPin

The pin that defines a local position and orientation on the first entity.

var pin1: GeometricPin

The pin that defines a local position and orientation on the second entity.

var tolerance: Float

An extension of the distance limit, as a percentage-based error tolerance.

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

struct PhysicsCustomJoint

A joint with six degrees of freedom that can be individually specified.

struct PhysicsFixedJoint

A joint that rigidly connects two entity pins, with zero degrees of freedom.

struct PhysicsJoints

A collection of physics joints.

