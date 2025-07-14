

- SpriteKit
-  SKPhysicsWorld 

Class

# SKPhysicsWorld

The driver of the physics engine in a scene; it exposes the ability for you to configure and query the physics system.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsWorld
```

## Mentioned in 

Disconnecting Bodies from Joints

Connecting Bodies with Joints

Getting Started with Physics

## Overview

`SKPhysicsWorld` runs the physics engine of a scene and is the place that contact detection occurs. Do not create a `SKPhysicsWorld` directly; the system creates a physics world and adds it to the scene’s physicsWorld property.

The physics world allows you to:

- Set important properties like gravity

- Join two physics bodies using an SKPhysicsJoint

- Respond to collision between two physics bodies using contactDelegate

- Do custom collisions detection or hit testing

## Topics

### Configuring the Physics World

var gravity: CGVector

A vector that specifies the gravitational acceleration applied to physics bodies in the physics world.

var speed: CGFloat

The rate at which the simulation executes.

### Joining Physics Bodies with Joints

func add(SKPhysicsJoint)

Adds a joint to the physics world.

func removeAllJoints()

Removes all joints from the physics world.

func remove(SKPhysicsJoint)

Removes a specific joint from the physics world.

### Detecting Collisions

var contactDelegate: (any SKPhysicsContactDelegate)?

A delegate that is called when two physics bodies come in contact with each other.

### Searching the Scene for Physics Bodies

Searching the World for Physics Bodies

Cast a ray to find the physics bodies in the scene that intersect it.

func body(alongRayStart: CGPoint, end: CGPoint) -> SKPhysicsBody?

Searches for the first physics body that intersects a ray.

func body(at: CGPoint) -> SKPhysicsBody?

Searches for the first physics body that contains a point.

func body(in: CGRect) -> SKPhysicsBody?

Searches for the first physics body that intersects the specified rectangle.

func enumerateBodies(alongRayStart: CGPoint, end: CGPoint, using: (SKPhysicsBody, CGPoint, CGVector, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect a ray.

func enumerateBodies(at: CGPoint, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that contain a point.

func enumerateBodies(in: CGRect, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect the specified rectangle.

### Sampling Physics Fields

func sampleFields(at: vector_float3) -> vector_float3

Samples all of the field nodes in the scene and returns the summation of their forces at that point.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Physics Simulation

Getting Started with Physics

Simulate gravity, acceleration, collision detection, or joints.

class SKPhysicsBody

An object that adds physics simulation to a node.

class SKPhysicsContact

A description of the contact between two physics bodies.

protocol SKPhysicsContactDelegate

Methods your app can implement to respond when physics bodies come into contact.

class SKFieldNode

A node that applies physics effects to nearby nodes.

