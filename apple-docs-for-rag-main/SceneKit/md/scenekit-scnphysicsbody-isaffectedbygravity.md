

- SceneKit
- SCNPhysicsBody
-  isAffectedByGravity 

Instance Property

# isAffectedByGravity

A Boolean value that determines whether the constant gravity of a scene accelerates the body.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isAffectedByGravity: Bool { get set }
```

## Discussion

If this property is true (the default), and the type of the body is SCNPhysicsBodyType.dynamic, the gravity property of the scene’s physicsWorld object causes the body to accelerate.

If this property is false, the body is not affected by scene gravity. This option can be useful when making physics bodies whose behavior should be governed by SCNPhysicsField objects instead of a constant global acceleration.

## See Also

### Defining How Forces Affect a Physics Body

var physicsShape: SCNPhysicsShape?

An object that defines the solid volume of the physics body for use in collision detection.

var type: SCNPhysicsBodyType

A constant that determines how the physics body responds to forces and collisions.

enum SCNPhysicsBodyType

Constants that determine how a physics body interacts with forces and other bodies, used by the type property and when creating a physics body.

var velocityFactor: SCNVector3

A multiplier affecting how SceneKit applies translations computed by the physics simulation to the node containing the physics body.

var angularVelocityFactor: SCNVector3

A multiplier affecting how SceneKit applies rotations computed by the physics simulation to the node containing the physics body.

