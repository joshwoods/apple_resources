

- SceneKit
- SCNParticleSystem
-  dampingFactor 

Instance Property

# dampingFactor

A factor that slows particles relative to their velocity. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var dampingFactor: CGFloat { get set }
```

## Discussion

Use this property to simulate effects such as fluid friction or air resistance on particles. A value of `0.0` (the default) specifies no slowing—that is, each particle maintains a constant speed (unless affected by gravity, acceleration, physics fields, or other influences). A value of `1.0` prevents particles from moving.

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

