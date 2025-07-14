

- SpriteKit
-  SKPhysicsJoint 

Class

# SKPhysicsJoint

The abstract superclass for objects that connect physics bodies.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsJoint
```

## Mentioned in 

Getting Started with Physics

## Overview

An SKPhysicsJoint object connects two physics bodies so that they are simulated together by the physics world. You never instantiate objects of this class directly; instead, you instantiate one of the subclasses that defines the kind of joint you want to make.

## Topics

### Connecting Bodies with Joints

Connecting Bodies with Joints

Add joints to nodes in your scene.

### Disconnecting Bodies from Joints

Disconnecting Bodies from Joints

Disconnect joints from nodes in your scene.

### Accessing or Setting a Joint’s Bodies

var bodyA: SKPhysicsBody

The first body connected by the joint.

var bodyB: SKPhysicsBody

The second body connected by the joint.

### Reading the Stress and Speed that Are Currently Applied to a Joint

var reactionForce: CGVector

The instantaneous reaction force, in newtons, currently being directed at the anchor point.

var reactionTorque: CGFloat

Instantaneous reaction torque, in newton-meters, currently being directed at the anchor point.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SKPhysicsJointFixed
- SKPhysicsJointLimit
- SKPhysicsJointPin
- SKPhysicsJointSliding
- SKPhysicsJointSpring

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

### Physics Joints

Working with Inverse Kinematics

Gain fine-tuned control of objects that are connected by joints.

class SKPhysicsJointFixed

A joint that fuses two physics bodies together at a reference point.

class SKPhysicsJointLimit

A joint that imposes a maximum distance between two physics bodies, as if they were connected by a rope.

class SKPhysicsJointPin

A joint that pins together two physics bodies, allowing independent rotation.

class SKPhysicsJointSliding

A joint that allows two physics bodies to slide along an axis.

class SKPhysicsJointSpring

A joint that simulates a spring connecting two physics bodies.

