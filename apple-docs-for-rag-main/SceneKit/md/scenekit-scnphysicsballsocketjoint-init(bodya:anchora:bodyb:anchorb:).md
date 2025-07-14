

- SceneKit
- SCNPhysicsBallSocketJoint
-  init(bodyA:anchorA:bodyB:anchorB:) 

Initializer

# init(bodyA:anchorA:bodyB:anchorB:)

Creates a ball and socket joint connecting two physics bodies.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    bodyA: SCNPhysicsBody,
    anchorA: SCNVector3,
    bodyB: SCNPhysicsBody,
    anchorB: SCNVector3
)
```

## Parameters 

`bodyA`  

The first physics body to be connected by the joint.

`anchorA`  

The point at which the joint connects, relative to the node containing the first body.

`bodyB`  

The second physics body to be connected by the joint.

`anchorB`  

The point at which the joint connects, relative to the node containing the second body.

## Return Value

A new ball-and-socket-joint behavior.

## Discussion

For a behavior to take effect, add it to the physics simulation by calling the addBehavior(_:) method on your scene’s SCNPhysicsWorld object. The physics bodies constrained by the joint must be attached to nodes in the scene.

## See Also

### Creating a Ball and Socket Joint

convenience init(body: SCNPhysicsBody, anchor: SCNVector3)

Creates a ball and socket joint that anchors a single physics body in space and allows it to rotate freely around an anchor point.

