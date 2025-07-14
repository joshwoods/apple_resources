

- SceneKit
-  SCNPhysicsConeTwistJoint 

Class

# SCNPhysicsConeTwistJoint

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class SCNPhysicsConeTwistJoint
```

## Topics

### Initializers

convenience init(body: SCNPhysicsBody, frame: SCNMatrix4)

convenience init(bodyA: SCNPhysicsBody, frameA: SCNMatrix4, bodyB: SCNPhysicsBody, frameB: SCNMatrix4)

### Instance Properties

var bodyA: SCNPhysicsBody

var bodyB: SCNPhysicsBody?

var frameA: SCNMatrix4

var frameB: SCNMatrix4

var maximumAngularLimit1: CGFloat

var maximumAngularLimit2: CGFloat

var maximumTwistAngle: CGFloat

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

class SCNPhysicsBallSocketJoint

A physics behavior that connects two physics bodies and allows them to pivot around each other in any direction.

