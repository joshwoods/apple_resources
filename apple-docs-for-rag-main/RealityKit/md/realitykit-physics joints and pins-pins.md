

- RealityKit
-  Physics joints and pins 

API Collection

# Physics joints and pins

Simulate joint physics that connect virtual objects.

## Overview

In a 3D environment, you can animate various attributes of an Entity such as its location, rotation, and size from one value to another. This is ideal for simple pre-defined motion, but does not allow for interaction with external forces, such as collisions with other objects, or gestures. With a PhysicsJoint you can connect entities with pins, and RealityKit keeps your entities bound by constraints that you define.

Each joint consists of two pins, each of which belongs to a different entity. Each GeometricPin moves and rotates relative to each other within the bounds of the joint’s constraints.

## Topics

### Pin and joint components

Simulating physics joints in your RealityKit app

Create realistic, connected motion using physics joints.

struct GeometricPin

A structure that identifies a local transform relative to an entity or entity’s animating skeletal joint.

struct GeometricPinsComponent

A component that stores a sequence of geometric pins.

protocol PhysicsJoint

A type that describes physics joints.

struct PhysicsJointsComponent

A component that stores physics joints which RealityKit simulates.

struct EntityGeometricPins

A structure that wraps all geometric pins an entity owns.

### Built-in joint types

struct PhysicsRevoluteJoint

A joint that allows one degree of rotational freedom between two entity pins, similar to a door swinging on its hinges.

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

## See Also

### Physics simulation

Collision detection

Determine when entities collide with each other or the environment.

Simulations and motion

Simulate physical interactions between entities or systems.

Force effects

Control the movement of virtual objects with forces.

