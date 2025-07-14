

- SpriteKit
-  SKPhysicsJointLimit 

Class

# SKPhysicsJointLimit

A joint that imposes a maximum distance between two physics bodies, as if they were connected by a rope.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsJointLimit
```

## Topics

### Creating a Limit Joint

class func joint(withBodyA: SKPhysicsBody, bodyB: SKPhysicsBody, anchorA: CGPoint, anchorB: CGPoint) -> SKPhysicsJointLimit

Creates a new limit joint.

### Configuring a Limit Joint

var maxLength: CGFloat

The maximum distance allowed between the two physics bodies connected by the limit joint.

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

class SKPhysicsJointPin

A joint that pins together two physics bodies, allowing independent rotation.

class SKPhysicsJointSliding

A joint that allows two physics bodies to slide along an axis.

class SKPhysicsJointSpring

A joint that simulates a spring connecting two physics bodies.

