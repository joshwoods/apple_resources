

- SpriteKit
-  SKPhysicsJointSpring 

Class

# SKPhysicsJointSpring

A joint that simulates a spring connecting two physics bodies.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsJointSpring
```

## Mentioned in 

Getting Started with Spring Joints

## Overview

An SKPhysicsJointSpring object simulates connecting two physics bodies together with a spring. The farther the two objects move from each other, the more force is applied to bring the two bodies back together.

## Topics

### First Steps

Getting Started with Spring Joints

Connect two physics bodies with a spring joint.

### Creating a Spring Joint

class func joint(withBodyA: SKPhysicsBody, bodyB: SKPhysicsBody, anchorA: CGPoint, anchorB: CGPoint) -> SKPhysicsJointSpring

Creates a new spring joint.

### Configuring a Spring Joint

var damping: CGFloat

Defines how the spring’s motion should be damped due to the forces of friction.

var frequency: CGFloat

Defines the frequency or stiffness characteristics of the spring.

## Relationships

### Inherits From

- SKPhysicsJoint

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

class SKPhysicsJoint

The abstract superclass for objects that connect physics bodies.

class SKPhysicsJointFixed

A joint that fuses two physics bodies together at a reference point.

class SKPhysicsJointLimit

A joint that imposes a maximum distance between two physics bodies, as if they were connected by a rope.

class SKPhysicsJointPin

A joint that pins together two physics bodies, allowing independent rotation.

class SKPhysicsJointSliding

A joint that allows two physics bodies to slide along an axis.

