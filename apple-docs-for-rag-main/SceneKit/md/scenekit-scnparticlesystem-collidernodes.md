

- SceneKit
- SCNParticleSystem
-  colliderNodes 

Instance Property

# colliderNodes

The nodes whose geometry the system’s particles can collide with.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var colliderNodes: [SCNNode]? { get set }
```

## Discussion

A particle system can perform limited collision detection and resolution with geometries in the scene. If a moving particle intersects a geometry attached to one of the SCNNode objects in this array, SceneKit resolves the collision, either by removing the particle from the scene or allowing it to bounce off or slide along the geometry’s surface.

Note

Collision detection is computationally intensive. For the best rendering performance, limit the number of collider nodes for each particle system, and use only simple geometries—represented by the SCNSphere, SCNPlane, and SCNFloor classes—as collision surfaces.

This array is empty by default.

## See Also

### Simulating Physics for Particles

var isAffectedByGravity: Bool

A Boolean value that determines whether gravity, as defined by the scene’s physics simulation, affects the motion of particles.

var isAffectedByPhysicsFields: Bool

A Boolean value that determines whether physics fields in the scene affect the motion of particles.

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

