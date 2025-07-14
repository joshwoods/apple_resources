

- SceneKit
- SCNParticleSystem
-  particleCharge 

Instance Property

# particleCharge

The electric charge, in coulombs, of each particle in the system. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleCharge: CGFloat { get set }
```

## Discussion

A particle’s charge determines its behavior when affected by an electric or magnetic field. Use the SCNPhysicsField class to add these fields to your scene. Particles with positive or negative charges behave differently when affected by electric or magnetic fields. (Note that while SceneKit uses SI units as the basis for its physics simulation, you need not worry about realism — experiment with different combinations of values to find the behavior that works best for your app or game.) You can randomize the charges of particles in the system with the particleChargeVariation property.

The default value is `0.0` coulombs, making the particle system unaffected by electric or magnetic fields.

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

var particleMassVariation: CGFloat

The range, in kilograms, of randomized particle masses. Animatable.

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

