

- SceneKit
- SCNPhysicsBallSocketJoint
-  anchorB 

Instance Property

# anchorB

The point at which the joint connects, relative to the node containing the second body.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var anchorB: SCNVector3 { get set }
```

## See Also

### Managing the Characteristics of a Ball and Socket Joint

var bodyA: SCNPhysicsBody

The first physics body connected by the joint.

var anchorA: SCNVector3

The point at which the joint connects, relative to the node containing the first body.

var bodyB: SCNPhysicsBody?

The second physics body connected by the joint.

