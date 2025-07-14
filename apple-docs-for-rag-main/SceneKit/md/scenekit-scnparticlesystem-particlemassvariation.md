

- SceneKit
- SCNParticleSystem
-  particleMassVariation 

Instance Property

# particleMassVariation

The range, in kilograms, of randomized particle masses. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleMassVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the particleMass property. SceneKit randomly adjusts the mass of each particle by up to half the particleMassVariation value. For example, if the particleMass value is `1.0` kilograms and the particleMassVariation value is `0.5` kilograms, each particle uses a random mass value between `0.75` and `1.25` kilograms for physics simulation.

The default value is `0.0` kilograms, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Simulating Physics for Particles

var isAffectedByGravity: Bool

A Boolean value that determines whether gravity, as defined by the scene’s physics simulation, affects the motion of particles.

var isAffectedByPhysicsFields: Bool

A Boolean value that determines whether physics fields in the scene affect the motion of particles.

var colliderNodes: [SCNNode]?

The nodes whose geometry the system’s particles can collide with.

var particleDiesOnCollision: Bool

A Boolean value that determines whether particles are removed from the scene upon colliding with another object.

var acceleration: SCNVector3

The constant acceleration vector, in units per second per second, applied to all particles in the system. Animatable.

var dampingFactor: CGFloat

A factor that slows particles relative to their velocity. Animatable.

var particleMass: CGFloat

The mass, in kilograms, of each particle in the system. Animatable.

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

