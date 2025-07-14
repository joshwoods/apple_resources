

- SceneKit
- SCNPhysicsSliderJoint
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

### Managing the Characteristics of a Slider Joint

var bodyA: SCNPhysicsBody

The first physics body connected by the joint.

var axisA: SCNVector3

The axis along which the first body can slide, relative to the node containing it.

var anchorA: SCNVector3

The point at which the joint connects, relative to the node containing the first body.

var axisB: SCNVector3

The axis along which the second body can slide, relative to the node containing it.

var anchorB: SCNVector3

The point at which the joint connects, relative to the node containing the second body.

