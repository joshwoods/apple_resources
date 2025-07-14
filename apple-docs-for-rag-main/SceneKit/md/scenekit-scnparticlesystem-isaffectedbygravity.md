

- SceneKit
- SCNParticleSystem
-  isAffectedByGravity 

Instance Property

# isAffectedByGravity

A Boolean value that determines whether gravity, as defined by the scene’s physics simulation, affects the motion of particles.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isAffectedByGravity: Bool { get set }
```

## Discussion

Gravity applies a constant acceleration to all particles in the system. SceneKit offers two options for simulating the effect of gravity on particles:

- The isAffectedByGravity property, which uses the gravity vector specified by the physicsWorld object of the scene containing the particle system. Use this option when you want the system’s particles to be affected by the same gravity as the SCNPhysicsBody objects in your scene.

- The acceleration property, which is independent of the simulation SceneKit uses for physics bodies in the scene. Use acceleration to simulate gravity if you have no SCNPhysicsBody objects in your scene, or if you want particles to be affected both by the physics world’s gravity and another constant acceleration (such as wind).

The default value is false, specifying that the physics world’s gravity does not affect particles.

## See Also

### Simulating Physics for Particles

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

