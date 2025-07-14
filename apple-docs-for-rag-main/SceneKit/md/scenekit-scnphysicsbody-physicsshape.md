

- SceneKit
- SCNPhysicsBody
-  physicsShape 

Instance Property

# physicsShape

An object that defines the solid volume of the physics body for use in collision detection.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var physicsShape: SCNPhysicsShape? { get set }
```

## Discussion

The physics simulation does not use a node’s visible geometry for collision detection—the simulation can run faster when using simple shapes, and it can also be useful to design your app or game using invisible collision shapes for some elements. Typically, you set a body’s physics shape to a bounding box or primitive shape that roughly matches its node’s visible content, but you can use a more detailed shape for more precise collision detection at a cost to performance.

For details on creating physics shapes, see SCNPhysicsShape.

## See Also

### Defining How Forces Affect a Physics Body

var type: SCNPhysicsBodyType

A constant that determines how the physics body responds to forces and collisions.

enum SCNPhysicsBodyType

Constants that determine how a physics body interacts with forces and other bodies, used by the type property and when creating a physics body.

var velocityFactor: SCNVector3

A multiplier affecting how SceneKit applies translations computed by the physics simulation to the node containing the physics body.

var angularVelocityFactor: SCNVector3

A multiplier affecting how SceneKit applies rotations computed by the physics simulation to the node containing the physics body.

var isAffectedByGravity: Bool

A Boolean value that determines whether the constant gravity of a scene accelerates the body.

