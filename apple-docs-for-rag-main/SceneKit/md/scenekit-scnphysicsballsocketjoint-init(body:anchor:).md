

- SceneKit
- SCNPhysicsBallSocketJoint
-  init(body:anchor:) 

Initializer

# init(body:anchor:)

Creates a ball and socket joint that anchors a single physics body in space and allows it to rotate freely around an anchor point.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    body: SCNPhysicsBody,
    anchor: SCNVector3
)
```

## Parameters 

`body`  

The physics body to be controlled by the joint.

`anchor`  

The point the body pivots around, relative to the node containing it.

## Return Value

A new ball-and-socket-joint behavior.

## Discussion

For a behavior to take effect, add it to the physics simulation by calling the addBehavior(_:) method on your scene’s SCNPhysicsWorld object. The physics bodies constrained by the joint must be attached to nodes in the scene.

## See Also

### Creating a Ball and Socket Joint

convenience init(bodyA: SCNPhysicsBody, anchorA: SCNVector3, bodyB: SCNPhysicsBody, anchorB: SCNVector3)

Creates a ball and socket joint connecting two physics bodies.

