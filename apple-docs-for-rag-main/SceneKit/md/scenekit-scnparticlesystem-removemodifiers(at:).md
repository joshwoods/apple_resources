

- SceneKit
- SCNParticleSystem
-  removeModifiers(at:) 

Instance Method

# removeModifiers(at:)

Removes particle modifier blocks for the specified stage of the particle simulation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func removeModifiers(at stage: SCNParticleModifierStage)
```

## Parameters 

`stage`  

The stage of SceneKit’s particle simulation during which to call the block. See SCNParticleModifierStage for allowed values.

## See Also

### Modifying Particles Over Time

var propertyControllers: [SCNParticleSystem.ParticleProperty : SCNParticlePropertyController]?

A dictionary that optionally associates particle properties with objects that animate a property’s value for each particle.

func addModifier(forProperties: [SCNParticleSystem.ParticleProperty], at: SCNParticleModifierStage, modifier: SCNParticleModifierBlock)

Adds a block that modifies particle properties, to be executed each time SceneKit renders a frame.

func removeAllModifiers()

Removes all particle modifier blocks associated with the particle system.

struct ParticleProperty

Keys identifying properties of individual particles, used by the propertyControllers dictionary and the handle(_:forProperties:handler:) and addModifier(forProperties:at:modifier:) methods.

enum SCNParticleModifierStage

Stages of SceneKit’s particle simulation process into which you can insert modifier blocks, used by the addModifier(forProperties:at:modifier:) method.

typealias SCNParticleModifierBlock

The signature for blocks called by SceneKit to modify particle properties on each frame of simulation, used by the addModifier(forProperties:at:modifier:) method.

