

- SceneKit
- SCNParticleSystem
-  handle(\_:forProperties:handler:) 

Instance Method

# handle(\_:forProperties:handler:)

Adds a block that modifies particle properties, to be executed at a specified event in the lifetimes of particles in the system.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func handle(
    _ event: SCNParticleEvent,
    forProperties properties: [SCNParticleSystem.ParticleProperty],
    handler block: @escaping SCNParticleEventBlock
)
```

## Parameters 

`event`  

The event at which to call the block. See SCNParticleEvent for allowed values.

`properties`  

An array containing one or more of the constants listed in `Particle Property Keys`, each of which specifies a property of the appearance or behaviors of particles in the particle system.

`block`  

A SCNParticleEventBlock block to be called every time SceneKit renders a frame. In this block you can modify the properties of particles in the system.

## Discussion

By associating a block with one or more particle properties, you can run arbitrary code that modifies those properties when a significant event in the particle simulation occurs for one or more particles. For example, you can use the following code with a confetti effect to randomly switch between two distinct colors for each spawned particle:

```
[system handleEvent:SCNParticleEventBirth
      forProperties:@[SCNParticlePropertyColor]
          withBlock:^(void **data, size_t *dataStride, uint32_t *indices , NSInteger count) {
              for (NSInteger i = 0; i 

## See Also

### Modifying Particles in Response to Particle System Events

enum SCNParticleEvent

Significant events in the life spans of simulate particles, used by the handle(_:forProperties:handler:) method.

typealias SCNParticleEventBlock

The signature for blocks called by SceneKit in response to significant events during particle simulation, used by the handle(_:forProperties:handler:) method.

