

- SceneKit
-  SCNPhysicsContactDelegate 

Protocol

# SCNPhysicsContactDelegate

Methods you can implement to respond when a contact or collision occurs between two physics bodies in a scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
protocol SCNPhysicsContactDelegate : NSObjectProtocol
```

## Overview

To receive contact messages, you set the contactDelegate property of an SCNPhysicsWorld object. SceneKit calls your delegate methods when a contact begins, when information about the contact changes, and when the contact ends.

## Topics

### Responding to Contact Events

func physicsWorld(SCNPhysicsWorld, didBegin: SCNPhysicsContact)

Tells the delegate that two bodies have come into contact.

func physicsWorld(SCNPhysicsWorld, didUpdate: SCNPhysicsContact)

Tells the delegate that new information is available about an ongoing contact.

func physicsWorld(SCNPhysicsWorld, didEnd: SCNPhysicsContact)

Tells the delegate that a contact has ended.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Collision and Contact Detection

class SCNPhysicsContact

Detailed information about a contact between two physics bodies in a scene’s physics simulation.

