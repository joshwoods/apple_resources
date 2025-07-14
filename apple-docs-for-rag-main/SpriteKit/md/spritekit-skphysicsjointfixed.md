

- SpriteKit
-  SKPhysicsJointFixed 

Class

# SKPhysicsJointFixed

A joint that fuses two physics bodies together at a reference point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsJointFixed
```

## Overview

An SKPhysicsJointFixed object fuses two physics bodies together at a reference point. Fixed joints are useful for creating complex shapes that can be broken apart later.

## Topics

### Creating a Fixed Joint

class func joint(withBodyA: SKPhysicsBody, bodyB: SKPhysicsBody, anchor: CGPoint) -> SKPhysicsJointFixed

Creates a new fixed joint.

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

class SKPhysicsJointLimit

A joint that imposes a maximum distance between two physics bodies, as if they were connected by a rope.

class SKPhysicsJointPin

A joint that pins together two physics bodies, allowing independent rotation.

class SKPhysicsJointSliding

A joint that allows two physics bodies to slide along an axis.

class SKPhysicsJointSpring

A joint that simulates a spring connecting two physics bodies.

