

- SceneKit
- SCNParticleSystem
-  addModifier(forProperties:at:modifier:) 

Instance Method

# addModifier(forProperties:at:modifier:)

Adds a block that modifies particle properties, to be executed each time SceneKit renders a frame.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func addModifier(
    forProperties properties: [SCNParticleSystem.ParticleProperty],
    at stage: SCNParticleModifierStage,
    modifier block: @escaping SCNParticleModifierBlock
)
```

## Parameters 

`properties`  

An array containing one or more of the constants listed in `Particle Property Keys`, each of which specifies a property of the appearance or behaviors of particles in the particle system.

`stage`  

The stage of SceneKit’s particle simulation during which to call the block. See SCNParticleModifierStage for allowed values.

`block`  

A SCNParticleModifierBlock block to be called every time SceneKit renders a frame. In this block you can modify the properties of all particles in the system.

## Discussion

By associating a block with one or more particle properties, you can run arbitrary code that modifies those properties during each frame of animation. This option provides maximum flexibility for changing the appearance or behavior of particles over time.

Important

Running your own code to update particle properties every frame can have a severe impact on rendering performance. If the behavior over time that you want for your particle system can be described more declaratively, use the propertyControllers property and SCNParticlePropertyController class instead. If you need to change particle properties only at certain times (rather than continuously), add a handler block for an event using the handle(_:forProperties:handler:) method.

## See Also

### Related Documentation

func handle(SCNParticleEvent, forProperties: [SCNParticleSystem.ParticleProperty], handler: SCNParticleEventBlock)

Adds a block that modifies particle properties, to be executed at a specified event in the lifetimes of particles in the system.

### Modifying Particles Over Time

var propertyControllers: [SCNParticleSystem.ParticleProperty : SCNParticlePropertyController]?

A dictionary that optionally associates particle properties with objects that animate a property’s value for each particle.

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

