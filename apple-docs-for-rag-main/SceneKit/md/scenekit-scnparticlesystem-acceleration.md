

- SceneKit
- SCNParticleSystem
-  acceleration 

Instance Property

# acceleration

The constant acceleration vector, in units per second per second, applied to all particles in the system. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var acceleration: SCNVector3 { get set }
```

## Discussion

Use this property to simulate effects such as wind or gravity on particles.

To use the same gravity vector that applies to physics bodies in the scene, or to apply more than one constant acceleration to particles, see the isAffectedByGravity property.

The default value is SCNVector3Zero, specifying no acceleration.

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

