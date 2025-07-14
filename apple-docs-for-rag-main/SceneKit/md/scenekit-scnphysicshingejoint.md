

- SceneKit
-  SCNPhysicsHingeJoint 

Class

# SCNPhysicsHingeJoint

A physics behavior that connects two bodies and allows them to pivot around each other on a single axis.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsHingeJoint
```

## Overview

A hinge has a single degree of freedom (rotation). You can also use a hinge joint to pin a body so that it can only move by rotating around a specific axis in the coordinate space of the node containing it.

## Topics

### Creating a Hinge Joint

convenience init(bodyA: SCNPhysicsBody, axisA: SCNVector3, anchorA: SCNVector3, bodyB: SCNPhysicsBody, axisB: SCNVector3, anchorB: SCNVector3)

Creates a hinge joint connecting two physics bodies.

convenience init(body: SCNPhysicsBody, axis: SCNVector3, anchor: SCNVector3)

Creates a hinge joint that anchors a single physics body in space and lets it rotate around a specific axis.

### Managing the Characteristics of a Hinge Joint

var bodyA: SCNPhysicsBody

The first physics body connected by the joint.

var axisA: SCNVector3

The axis that the hinge pivots around, relative to the node containing the first body.

var anchorA: SCNVector3

The point at which the hinge connects, relative to the node containing the first body.

var bodyB: SCNPhysicsBody?

The second physics body connected by the joint.

var axisB: SCNVector3

The axis that the hinge pivots around, relative to the node containing the second body.

var anchorB: SCNVector3

The point at which the hinge connects, relative to the node containing the second body.

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

class SCNPhysicsSliderJoint

A physics behavior that connects two bodies and allows them to slide against each other and rotate around their connecting points.

class SCNPhysicsBallSocketJoint

A physics behavior that connects two physics bodies and allows them to pivot around each other in any direction.

class SCNPhysicsConeTwistJoint

