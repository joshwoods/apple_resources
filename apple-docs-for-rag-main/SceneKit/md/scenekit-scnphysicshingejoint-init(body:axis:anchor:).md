

- SceneKit
- SCNPhysicsHingeJoint
-  init(body:axis:anchor:) 

Initializer

# init(body:axis:anchor:)

Creates a hinge joint that anchors a single physics body in space and lets it rotate around a specific axis.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    body: SCNPhysicsBody,
    axis: SCNVector3,
    anchor: SCNVector3
)
```

## Parameters 

`body`  

The physics body to be controlled by the hinge joint.

`axis`  

The direction of the axis that the body pivots around, relative to the node containing the body.

`anchor`  

The location of the axis in the node containing the body.

## Return Value

A new hinge joint behavior.

## Discussion

For a behavior to take effect, add it to the physics simulation by calling the addBehavior(_:) method on your scene’s SCNPhysicsWorld object. The physics bodies constrained by the joint must be attached to nodes in the scene.

## See Also

### Creating a Hinge Joint

convenience init(bodyA: SCNPhysicsBody, axisA: SCNVector3, anchorA: SCNVector3, bodyB: SCNPhysicsBody, axisB: SCNVector3, anchorB: SCNVector3)

Creates a hinge joint connecting two physics bodies.

