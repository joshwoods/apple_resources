

- SceneKit
- SCNPhysicsBallSocketJoint
-  bodyA 

Instance Property

# bodyA

The first physics body connected by the joint.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var bodyA: SCNPhysicsBody { get }
```

## See Also

### Managing the Characteristics of a Ball and Socket Joint

var anchorA: SCNVector3

The point at which the joint connects, relative to the node containing the first body.

var bodyB: SCNPhysicsBody?

The second physics body connected by the joint.

var anchorB: SCNVector3

The point at which the joint connects, relative to the node containing the second body.

