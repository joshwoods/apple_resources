

- SceneKit
- SCNPhysicsHingeJoint
-  init(bodyA:axisA:anchorA:bodyB:axisB:anchorB:) 

Initializer

# init(bodyA:axisA:anchorA:bodyB:axisB:anchorB:)

Creates a hinge joint connecting two physics bodies.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    bodyA: SCNPhysicsBody,
    axisA: SCNVector3,
    anchorA: SCNVector3,
    bodyB: SCNPhysicsBody,
    axisB: SCNVector3,
    anchorB: SCNVector3
)
```

## Parameters 

`bodyA`  

The first physics body to be connected by the joint.

`axisA`  

The axis that the hinge pivots around, relative to the node containing the first body.

`anchorA`  

The point at which the hinge connects, relative to the node containing the first body.

`bodyB`  

The second physics body to be connected by the joint.

`axisB`  

The axis that the hinge pivots around, relative to the node containing the second body.

`anchorB`  

The point at which the hinge connects, relative to the node containing the second body.

## Return Value

A new hinge joint behavior.

## Discussion

For a behavior to take effect, add it to the physics simulation by calling the addBehavior(_:) method on your scene’s SCNPhysicsWorld object. The physics bodies constrained by the joint must be attached to nodes in the scene.

## See Also

### Creating a Hinge Joint

convenience init(body: SCNPhysicsBody, axis: SCNVector3, anchor: SCNVector3)

Creates a hinge joint that anchors a single physics body in space and lets it rotate around a specific axis.

