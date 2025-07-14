

- SpriteKit
- SKPhysicsJointPin
-  joint(withBodyA:bodyB:anchor:) 

Type Method

# joint(withBodyA:bodyB:anchor:)

Creates a new pin joint.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func joint(
    withBodyA bodyA: SKPhysicsBody,
    bodyB: SKPhysicsBody,
    anchor: CGPoint
) -> SKPhysicsJointPin
```

## Parameters 

`bodyA`  

The first body to connect. The body must be connected to a node that is already part of the scene’s node tree.

`bodyB`  

The second body to connect. The body must be connected to a node that is already part of the scene’s node tree.

`anchor`  

The connection point between the two bodies in the scene’s coordinate system.

## Return Value

A new pin joint.

## Discussion

You must add the joint to a physics world associated with the scene before it takes effect.

