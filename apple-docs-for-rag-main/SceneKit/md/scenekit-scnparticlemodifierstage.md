

- SceneKit
-  SCNParticleModifierStage 

Enumeration

# SCNParticleModifierStage

Stages of SceneKit’s particle simulation process into which you can insert modifier blocks, used by the addModifier(forProperties:at:modifier:) method.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleModifierStage
```

## Topics

### Constants

case preDynamics

The stage before SceneKit simulates the motion of particles.

case postDynamics

The stage after SceneKit simulates the motion of particles.

case preCollision

The stage before SceneKit simulates the results of collisions between particles and scene geometry.

case postCollision

The stage after SceneKit simulates the results of collisions between particles and scene geometry.

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

### Modifying Particles Over Time

var propertyControllers: [SCNParticleSystem.ParticleProperty : SCNParticlePropertyController]?

A dictionary that optionally associates particle properties with objects that animate a property’s value for each particle.

func addModifier(forProperties: [SCNParticleSystem.ParticleProperty], at: SCNParticleModifierStage, modifier: SCNParticleModifierBlock)

Adds a block that modifies particle properties, to be executed each time SceneKit renders a frame.

func removeModifiers(at: SCNParticleModifierStage)

Removes particle modifier blocks for the specified stage of the particle simulation.

func removeAllModifiers()

Removes all particle modifier blocks associated with the particle system.

struct ParticleProperty

Keys identifying properties of individual particles, used by the propertyControllers dictionary and the handle(_:forProperties:handler:) and addModifier(forProperties:at:modifier:) methods.

typealias SCNParticleModifierBlock

The signature for blocks called by SceneKit to modify particle properties on each frame of simulation, used by the addModifier(forProperties:at:modifier:) method.

