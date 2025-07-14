

- SceneKit
- SCNParticleSystem
-  particleDiesOnCollision 

Instance Property

# particleDiesOnCollision

A Boolean value that determines whether particles are removed from the scene upon colliding with another object.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleDiesOnCollision: Bool { get set }
```

## Discussion

This property has no effect if the colliderNodes array is empty or contains no nodes with attached geometry.

The default value is false, specifying that particles remain in the scene after a collision. The particleBounce and particleFriction properties determine whether and how particles bounce or slide after colliding with a geometry.

## See Also

### Simulating Physics for Particles

var isAffectedByGravity: Bool

A Boolean value that determines whether gravity, as defined by the scene’s physics simulation, affects the motion of particles.

var isAffectedByPhysicsFields: Bool

A Boolean value that determines whether physics fields in the scene affect the motion of particles.

var colliderNodes: [SCNNode]?

The nodes whose geometry the system’s particles can collide with.

var acceleration: SCNVector3

The constant acceleration vector, in units per second per second, applied to all particles in the system. Animatable.

var dampingFactor: CGFloat

A factor that slows particles relative to their velocity. Animatable.

var particleMass: CGFloat

The mass, in kilograms, of each particle in the system. Animatable.

var particleMassVariation: CGFloat

The range, in kilograms, of randomized particle masses. Animatable.

var particleCharge: CGFloat

The electric charge, in coulombs, of each particle in the system. Animatable.

var particleChargeVariation: CGFloat

The range, in coulombs, of randomized particle charges. Animatable.

var particleBounce: CGFloat

The restitution coefficient of each particle in the system. Animatable.

var particleBounceVariation: CGFloat

The range of randomized restitution coefficients for particles. Animatable.

var particleFriction: CGFloat

The friction coefficient of each particle in the system. Animatable.

var particleFrictionVariation: CGFloat

The range of randomized friction coefficients for particles. Animatable.

