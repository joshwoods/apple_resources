

- SceneKit
- SCNParticleSystem
-  SCNParticleSystem.ParticleProperty 

Structure

# SCNParticleSystem.ParticleProperty

Keys identifying properties of individual particles, used by the propertyControllers dictionary and the handle(_:forProperties:handler:) and addModifier(forProperties:at:modifier:) methods.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct ParticleProperty
```

## Topics

### Type Properties

static let angle: SCNParticleSystem.ParticleProperty

The rotation angle, in radians, of the particle about its axis.

static let angularVelocity: SCNParticleSystem.ParticleProperty

The particle’s angular velocity (or rate of spin), in radians per second.

static let bounce: SCNParticleSystem.ParticleProperty

The particle’s restitution coefficient.

static let charge: SCNParticleSystem.ParticleProperty

The particle’s electric charge, in coulombs.

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

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying Particles Over Time

var propertyControllers: [SCNParticleSystem.ParticleProperty : SCNParticlePropertyController]?

A dictionary that optionally associates particle properties with objects that animate a property’s value for each particle.

func addModifier(forProperties: [SCNParticleSystem.ParticleProperty], at: SCNParticleModifierStage, modifier: SCNParticleModifierBlock)

Adds a block that modifies particle properties, to be executed each time SceneKit renders a frame.

func removeModifiers(at: SCNParticleModifierStage)

Removes particle modifier blocks for the specified stage of the particle simulation.

func removeAllModifiers()

Removes all particle modifier blocks associated with the particle system.

enum SCNParticleModifierStage

Stages of SceneKit’s particle simulation process into which you can insert modifier blocks, used by the addModifier(forProperties:at:modifier:) method.

typealias SCNParticleModifierBlock

The signature for blocks called by SceneKit to modify particle properties on each frame of simulation, used by the addModifier(forProperties:at:modifier:) method.

