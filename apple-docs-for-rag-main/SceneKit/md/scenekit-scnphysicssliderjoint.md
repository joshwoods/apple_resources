

- SceneKit
-  SCNPhysicsSliderJoint 

Class

# SCNPhysicsSliderJoint

A physics behavior that connects two bodies and allows them to slide against each other and rotate around their connecting points.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsSliderJoint
```

## Overview

A slider joint can have zero, one, or two degrees of freedom depending on whether you allow it to slide or rotate. You can also use a slider joint to pin a body so that it can move only by sliding a specific axis in the coordinate space of the node containing it. You can also use a slider joint as a motor, applying a force or torque to the bodies it connects.

## Topics

### Creating a Slider Joint

convenience init(bodyA: SCNPhysicsBody, axisA: SCNVector3, anchorA: SCNVector3, bodyB: SCNPhysicsBody, axisB: SCNVector3, anchorB: SCNVector3)

Creates a slider joint connecting two physics bodies.

convenience init(body: SCNPhysicsBody, axis: SCNVector3, anchor: SCNVector3)

Creates a slider joint that anchors a single physics body in space and allows it to slide along a specific axis.

### Managing the Characteristics of a Slider Joint

var bodyA: SCNPhysicsBody

The first physics body connected by the joint.

var axisA: SCNVector3

The axis along which the first body can slide, relative to the node containing it.

var anchorA: SCNVector3

The point at which the joint connects, relative to the node containing the first body.

var bodyB: SCNPhysicsBody?

The second physics body connected by the joint.

var axisB: SCNVector3

The axis along which the second body can slide, relative to the node containing it.

var anchorB: SCNVector3

The point at which the joint connects, relative to the node containing the second body.

### Limiting the Motion of a Slider Joint

var minimumLinearLimit: CGFloat

The minimum distance between the anchor points of the two bodies, relative to their initial positions.

var maximumLinearLimit: CGFloat

The maximum distance between the anchor points of the two bodies, relative to their initial positions.

var minimumAngularLimit: CGFloat

The minimum rotation angle between the two bodies, measured in radians relative to their initial orientations.

var maximumAngularLimit: CGFloat

The maximum rotation angle between the two bodies, measured in radians relative to their initial orientations.

### Applying Forces and Torques

var motorTargetLinearVelocity: CGFloat

The velocity at which the joint’s connected bodies should slide.

var motorMaximumForce: CGFloat

The maximum linear force that the joint can apply to its connected bodies, in newtons.

var motorTargetAngularVelocity: CGFloat

The angular velocity at which the joint’s connected bodies should rotate around it.

var motorMaximumTorque: CGFloat

The maximum torque that the joint can apply to its connected bodies, in newton-meters.

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

class SCNPhysicsBallSocketJoint

A physics behavior that connects two physics bodies and allows them to pivot around each other in any direction.

class SCNPhysicsConeTwistJoint

