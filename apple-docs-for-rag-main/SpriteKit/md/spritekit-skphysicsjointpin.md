

- SpriteKit
-  SKPhysicsJointPin 

Class

# SKPhysicsJointPin

A joint that pins together two physics bodies, allowing independent rotation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsJointPin
```

## Mentioned in 

Pinning and Rotating Physics Bodies

Connecting Bodies with Joints

## Overview

An SKPhysicsJointPin object allows two physics bodies to independently rotate around the anchor point as if pinned together. You can configure how far the two objects may rotate and the resistance to rotation.

## Topics

### Creating a Pin Joint

class func joint(withBodyA: SKPhysicsBody, bodyB: SKPhysicsBody, anchor: CGPoint) -> SKPhysicsJointPin

Creates a new pin joint.

### Configuring a Pin Joint

var rotationSpeed: CGFloat

The speed, in radians per second, at which the physics bodies are driven around the pin joint.

var shouldEnableLimits: Bool

A Boolean value that indicates whether the pin joint’s rotation is limited to a specific range of values.

var lowerAngleLimit: CGFloat

The smallest angle allowed for the pin joint, in radians.

var upperAngleLimit: CGFloat

The largest angle allowed for the pin joint, in radians.

var frictionTorque: CGFloat

The resistance applied by the pin joint to spinning around the anchor point.

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

class SKPhysicsJointSliding

A joint that allows two physics bodies to slide along an axis.

class SKPhysicsJointSpring

A joint that simulates a spring connecting two physics bodies.

