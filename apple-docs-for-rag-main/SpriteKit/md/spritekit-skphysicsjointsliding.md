

- SpriteKit
-  SKPhysicsJointSliding 

Class

# SKPhysicsJointSliding

A joint that allows two physics bodies to slide along an axis.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsJointSliding
```

## Overview

An SKPhysicsJointSliding object allows the anchor points of the two physics bodies to slide along a chosen axis. The joint can be configured to limit the distance that the two objects are allowed to slide along the axis.

## Topics

### Creating a Sliding Joint

class func joint(withBodyA: SKPhysicsBody, bodyB: SKPhysicsBody, anchor: CGPoint, axis: CGVector) -> SKPhysicsJointSliding

Creates a new sliding joint.

### Configuring a Sliding Joint

var shouldEnableLimits: Bool

A Boolean value that indicates whether the sliding joint is restricted so that the objects may only slide a finite distance from the initial anchor point.

var lowerDistanceLimit: CGFloat

The smallest distance allowed for the sliding joint.

var upperDistanceLimit: CGFloat

The largest distance allowed for the sliding joint.

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

class SKPhysicsJointSpring

A joint that simulates a spring connecting two physics bodies.

