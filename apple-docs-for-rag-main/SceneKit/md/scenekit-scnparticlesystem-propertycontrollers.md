

- SceneKit
- SCNParticleSystem
-  propertyControllers 

Instance Property

# propertyControllers

A dictionary that optionally associates particle properties with objects that animate a property’s value for each particle.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var propertyControllers: [SCNParticleSystem.ParticleProperty : SCNParticlePropertyController]? { get set }
```

## Discussion

Each key in this dictionary is one of the constants listed in `Particle Property Keys`, and the value for each key is a SCNParticlePropertyController object responsible for varying that property over time. Use particle property controllers to add efficient animations that change the appearance or behavior of each particle emitted by the system.

To add more complex behavior that cannot be described by a SCNParticlePropertyController object, use the addModifier(forProperties:at:modifier:) to add a particle modifier block. However, be aware that particle modifier blocks can severely impact rendering performance.

## See Also

### Modifying Particles Over Time

func addModifier(forProperties: [SCNParticleSystem.ParticleProperty], at: SCNParticleModifierStage, modifier: SCNParticleModifierBlock)

Adds a block that modifies particle properties, to be executed each time SceneKit renders a frame.

func removeModifiers(at: SCNParticleModifierStage)

Removes particle modifier blocks for the specified stage of the particle simulation.

func removeAllModifiers()

Removes all particle modifier blocks associated with the particle system.

struct ParticleProperty

Keys identifying properties of individual particles, used by the propertyControllers dictionary and the handle(_:forProperties:handler:) and addModifier(forProperties:at:modifier:) methods.

enum SCNParticleModifierStage

Stages of SceneKit’s particle simulation process into which you can insert modifier blocks, used by the addModifier(forProperties:at:modifier:) method.

typealias SCNParticleModifierBlock

The signature for blocks called by SceneKit to modify particle properties on each frame of simulation, used by the addModifier(forProperties:at:modifier:) method.

