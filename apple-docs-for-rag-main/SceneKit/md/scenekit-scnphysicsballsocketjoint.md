

- SceneKit
-  SCNPhysicsBallSocketJoint 

Class

# SCNPhysicsBallSocketJoint

A physics behavior that connects two physics bodies and allows them to pivot around each other in any direction.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsBallSocketJoint
```

## Overview

A ball and socket joint has three rotational degrees of freedom and zero translational degrees of freedom. You can also use a ball and socket joint to pin a body to a specific location in the coordinate space of the node containing it while allowing it to rotate freely.

## Topics

### Creating a Ball and Socket Joint

convenience init(bodyA: SCNPhysicsBody, anchorA: SCNVector3, bodyB: SCNPhysicsBody, anchorB: SCNVector3)

Creates a ball and socket joint connecting two physics bodies.

convenience init(body: SCNPhysicsBody, anchor: SCNVector3)

Creates a ball and socket joint that anchors a single physics body in space and allows it to rotate freely around an anchor point.

### Managing the Characteristics of a Ball and Socket Joint

var bodyA: SCNPhysicsBody

The first physics body connected by the joint.

var anchorA: SCNVector3

The point at which the joint connects, relative to the node containing the first body.

var bodyB: SCNPhysicsBody?

The second physics body connected by the joint.

var anchorB: SCNVector3

The point at which the joint connects, relative to the node containing the second body.

## Relationships

### Inherits From

- SCNPhysicsBehavior

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

### Joints

class SCNPhysicsHingeJoint

A physics behavior that connects two bodies and allows them to pivot around each other on a single axis.

class SCNPhysicsSliderJoint

A physics behavior that connects two bodies and allows them to slide against each other and rotate around their connecting points.

class SCNPhysicsConeTwistJoint

