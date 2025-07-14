

- SceneKit
- SCNPhysicsBody
-  velocityFactor 

Instance Property

# velocityFactor

A multiplier affecting how SceneKit applies translations computed by the physics simulation to the node containing the physics body.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var velocityFactor: SCNVector3 { get set }
```

## Discussion

Use this property to constrain or restrict the effect of physics simulation on the node containing the physics body. For example, you can force a body to move in only two dimensions by setting its velocity factor to `{1.0, 1.0, 0.0}`.

## See Also

### Defining How Forces Affect a Physics Body

var physicsShape: SCNPhysicsShape?

An object that defines the solid volume of the physics body for use in collision detection.

var type: SCNPhysicsBodyType

A constant that determines how the physics body responds to forces and collisions.

enum SCNPhysicsBodyType

Constants that determine how a physics body interacts with forces and other bodies, used by the type property and when creating a physics body.

var angularVelocityFactor: SCNVector3

A multiplier affecting how SceneKit applies rotations computed by the physics simulation to the node containing the physics body.

var isAffectedByGravity: Bool

A Boolean value that determines whether the constant gravity of a scene accelerates the body.

