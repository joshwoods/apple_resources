

- SceneKit
- SCNPhysicsHingeJoint
-  anchorB 

Instance Property

# anchorB

The point at which the hinge connects, relative to the node containing the second body.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var anchorB: SCNVector3 { get set }
```

## See Also

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

