

- SceneKit
- SCNParticleSystem
- SCNParticleSystem.ParticleProperty
-  charge 

Type Property

# charge

The particle’s electric charge, in coulombs.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let charge: SCNParticleSystem.ParticleProperty
```

## Discussion

This property’s value is a floating-point scalar (an NSNumber object for particle property controllers, or a single `float` value for particle event or modifier blocks). A particle’s charge determines its behavior when affected by an electric or magnetic field created with the SCNPhysicsField class.

The particle system’s particleCharge and particleChargeVariation properties determine the initial charge for each particle.

## See Also

### Type Properties

static let angle: SCNParticleSystem.ParticleProperty

The rotation angle, in radians, of the particle about its axis.

static let angularVelocity: SCNParticleSystem.ParticleProperty

The particle’s angular velocity (or rate of spin), in radians per second.

static let bounce: SCNParticleSystem.ParticleProperty

The particle’s restitution coefficient.

static let color: SCNParticleSystem.ParticleProperty

The particle’s tint color, as a vector of red, green, blue, and alpha component values.

static let contactNormal: SCNParticleSystem.ParticleProperty

The normal vector, in scene coordinate space, of a collision between a particle and a geometry in the scene.

static let contactPoint: SCNParticleSystem.ParticleProperty

The location, in scene coordinate space, of a collision between a particle and a geometry in the scene.

static let frame: SCNParticleSystem.ParticleProperty

The current frame index of the particle’s image animation.

static let frameRate: SCNParticleSystem.ParticleProperty

The rate, in frames per second, of the particle’s image animation.

static let friction: SCNParticleSystem.ParticleProperty

The particle’s friction coefficient.

static let life: SCNParticleSystem.ParticleProperty

The remaining time in the particle’s life span, in seconds.

static let opacity: SCNParticleSystem.ParticleProperty

The particle’s opacity (or alpha value).

static let position: SCNParticleSystem.ParticleProperty

The particle’s position vector in scene coordinate space.

static let rotationAxis: SCNParticleSystem.ParticleProperty

The particle’s axis of rotation, expressed as a vector in the particle’s local coordinate space.

static let size: SCNParticleSystem.ParticleProperty

The width and height of the rendered particle image, in units of scene coordinate space.

static let velocity: SCNParticleSystem.ParticleProperty

The particle’s velocity vector in units (of scene coordinate space) per second.

