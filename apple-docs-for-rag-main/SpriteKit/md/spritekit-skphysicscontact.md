

- SpriteKit
-  SKPhysicsContact 

Class

# SKPhysicsContact

A description of the contact between two physics bodies.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsContact
```

## Overview

An SKPhysicsContact object is created automatically by SpriteKit to describe a contact between two physical bodies in a physics world.To receive contact messages, read the physicsWorld property of an SKScene object you are interested in, and assign its contactDelegate property to point to an object that implements the SKPhysicsContactDelegate protocol. Then, for each physics body in your scene, set the categoryBitMask and contactTestBitMask properties to define which interactions should generate contact messages.

## Topics

### Inspecting the Contact Properties

var bodyA: SKPhysicsBody

The first body in the contact.

var bodyB: SKPhysicsBody

The second body in the contact.

var contactPoint: CGPoint

The contact point between the two physics bodies, in scene coordinates.

var collisionImpulse: CGFloat

The impulse that specifies how hard these two bodies struck each other in Newton-seconds.

var contactNormal: CGVector

The normal vector specifying the direction of the collision.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Physics Simulation

Getting Started with Physics

Simulate gravity, acceleration, collision detection, or joints.

class SKPhysicsWorld

The driver of the physics engine in a scene; it exposes the ability for you to configure and query the physics system.

class SKPhysicsBody

An object that adds physics simulation to a node.

protocol SKPhysicsContactDelegate

Methods your app can implement to respond when physics bodies come into contact.

class SKFieldNode

A node that applies physics effects to nearby nodes.

