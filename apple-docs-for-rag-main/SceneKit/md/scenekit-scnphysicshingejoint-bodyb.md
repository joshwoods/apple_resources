

- SceneKit
- SCNPhysicsHingeJoint
-  bodyB 

Instance Property

# bodyB

The second physics body connected by the joint.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var bodyB: SCNPhysicsBody? { get }
```

## Discussion

This property’s value is `nil` if the joint was created using the init(body:axis:anchor:) method.

## See Also

### Managing the Characteristics of a Hinge Joint

var bodyA: SCNPhysicsBody

The first physics body connected by the joint.

var axisA: SCNVector3

The axis that the hinge pivots around, relative to the node containing the first body.

var anchorA: SCNVector3

The point at which the hinge connects, relative to the node containing the first body.

var axisB: SCNVector3

The axis that the hinge pivots around, relative to the node containing the second body.

var anchorB: SCNVector3

The point at which the hinge connects, relative to the node containing the second body.

