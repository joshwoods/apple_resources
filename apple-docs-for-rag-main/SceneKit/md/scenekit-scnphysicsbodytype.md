

- SceneKit
-  SCNPhysicsBodyType 

Enumeration

# SCNPhysicsBodyType

Constants that determine how a physics body interacts with forces and other bodies, used by the type property and when creating a physics body.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNPhysicsBodyType
```

## Topics

### Constants

case `static`

A physics body that is unaffected by forces or collisions and cannot move.

case dynamic

A physics body that can be affected by forces and collisions.

case kinematic

A physics body that is unaffected by forces or collisions but that can cause collisions affecting other bodies when moved.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Defining How Forces Affect a Physics Body

var physicsShape: SCNPhysicsShape?

An object that defines the solid volume of the physics body for use in collision detection.

var type: SCNPhysicsBodyType

A constant that determines how the physics body responds to forces and collisions.

var velocityFactor: SCNVector3

A multiplier affecting how SceneKit applies translations computed by the physics simulation to the node containing the physics body.

var angularVelocityFactor: SCNVector3

A multiplier affecting how SceneKit applies rotations computed by the physics simulation to the node containing the physics body.

var isAffectedByGravity: Bool

A Boolean value that determines whether the constant gravity of a scene accelerates the body.

