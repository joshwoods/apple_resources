

- SceneKit
-  SCNPhysicsContact 

Class

# SCNPhysicsContact

Detailed information about a contact between two physics bodies in a scene’s physics simulation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsContact
```

## Overview

You don’t create SCNPhysicsContact instances directly; SceneKit automatically creates these objects whenever contacts occur.

To receive contact messages, assign your custom class implementing the SCNPhysicsContactDelegate protocol to the contactDelegate property of your scene’s SCNPhysicsWorld obejct. Next, for each physics body in your scene, set the categoryBitMask and collisionBitMask properties to define which interactions should generate contact messages.

## Topics

### Inspecting the Contact Properties

var nodeA: SCNNode

The node containing the first body in the contact.

var nodeB: SCNNode

The node containing the second body in the contact.

var contactPoint: SCNVector3

The contact point between the two physics bodies, in scene coordinates.

var contactNormal: SCNVector3

The normal vector at the contact point between the two physics bodies, in scene coordinates.

var collisionImpulse: CGFloat

The force over time of the collision, in newton-seconds.

var penetrationDistance: CGFloat

The distance of overlap, in units of scene coordinate space, between the two physics bodies.

### Instance Properties

var sweepTestFraction: CGFloat

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

### Collision and Contact Detection

protocol SCNPhysicsContactDelegate

Methods you can implement to respond when a contact or collision occurs between two physics bodies in a scene.

