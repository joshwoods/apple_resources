

- SceneKit
- SCNPhysicsSliderJoint
-  init(bodyA:axisA:anchorA:bodyB:axisB:anchorB:) 

Initializer

# init(bodyA:axisA:anchorA:bodyB:axisB:anchorB:)

Creates a slider joint connecting two physics bodies.

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

The axis along which the first body can slide, relative to the node containing it.

`anchorA`  

The point at which the joint connects, relative to the node containing the first body.

`bodyB`  

The second physics body to be connected by the joint.

`axisB`  

The axis along which the second body can slide, relative to the node containing it.

`anchorB`  

The point at which the joint connects, relative to the node containing the second body.

## Return Value

A new slider joint behavior.

## Discussion

This method defines the location where the bodies are pinned together. To define their sliding or rotation motion relative to that point, use the properties listed in Limiting the Motion of a Slider Joint.

For a behavior to take effect, add it to the physics simulation by calling the addBehavior(_:) method on your scene’s SCNPhysicsWorld object. The physics bodies constrained by the joint must be attached to nodes in the scene.

## See Also

### Creating a Slider Joint

convenience init(body: SCNPhysicsBody, axis: SCNVector3, anchor: SCNVector3)

Creates a slider joint that anchors a single physics body in space and allows it to slide along a specific axis.

