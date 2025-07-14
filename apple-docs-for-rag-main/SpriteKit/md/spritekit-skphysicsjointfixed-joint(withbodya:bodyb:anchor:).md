

- SpriteKit
- SKPhysicsJointFixed
-  joint(withBodyA:bodyB:anchor:) 

Type Method

# joint(withBodyA:bodyB:anchor:)

Creates a new fixed joint.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func joint(
    withBodyA bodyA: SKPhysicsBody,
    bodyB: SKPhysicsBody,
    anchor: CGPoint
) -> SKPhysicsJointFixed
```

## Parameters 

`bodyA`  

The first body to connect. The body must be connected to a node that is already part of the scene’s node tree.

`bodyB`  

The second body to connect. The body must be connected to a node that is already part of the scene’s node tree.

`anchor`  

The anchor point for the connection in the scene’s coordinate system.

## Return Value

A new fixed joint.

## Discussion

You must add the joint to a physics world associated with the scene before it takes effect.

