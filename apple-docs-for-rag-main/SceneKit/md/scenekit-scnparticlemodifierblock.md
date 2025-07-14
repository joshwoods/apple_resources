

- SceneKit
-  SCNParticleModifierBlock 

Type Alias

# SCNParticleModifierBlock

The signature for blocks called by SceneKit to modify particle properties on each frame of simulation, used by the addModifier(forProperties:at:modifier:) method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNParticleModifierBlock = (UnsafeMutablePointer, UnsafeMutablePointer, Int, Int, Float) -> Void
```

## Discussion

The block takes the following parameters:

data  
An array of floating-point values containing stripes of property data for the system’s particles. The width and format of each data stripe depend on the properties you specify when calling the addModifier(forProperties:at:modifier:) method.

dataStride  
An array identifying the offset, in bytes, of each property’s value in the data stripe for each particle. The order of offsets in this array corresponds to the order of the `properties` array you specify when calling the addModifier(forProperties:at:modifier:) method.

start  
The index of the first particle’s data stripe in the `data` array.

end  
The index of the last particle’s data stripe in the `data` array.

deltaTime  
The elapsed time, in seconds, since the last frame of simulation.

Use this block to change properties of individual particles on each frame of simulation.

Important

Running your own code to update particle properties every frame can have a severe impact on rendering performance. If the behavior over time that you want for your particle system can be described more declaratively, use the propertyControllers property and SCNParticlePropertyController class instead. If you need to change particle properties only at certain times (rather than continuously), add a handler block for an event using the handle(_:forProperties:handler:) method.

The following example illustrates setting up a modifier block that alters particle’s position and velocity:

```
[system addModifierForProperties:@[SCNParticlePropertyPosition,
                                   SCNParticlePropertyVelocity]
                         atStage:SCNParticleModifierStagePostDynamics
                       withBlock:^(void **data, size_t *dataStride, NSInteger start, NSInteger end, float deltaTime) {
                           // For each particle to be processed,
                           // calculate pointers in the data to each property's value:
                           for (NSInteger i = start; i 

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

enum SCNParticleModifierStage

Stages of SceneKit’s particle simulation process into which you can insert modifier blocks, used by the addModifier(forProperties:at:modifier:) method.

