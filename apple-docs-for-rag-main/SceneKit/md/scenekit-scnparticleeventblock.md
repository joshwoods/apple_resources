

- SceneKit
-  SCNParticleEventBlock 

Type Alias

# SCNParticleEventBlock

The signature for blocks called by SceneKit in response to significant events during particle simulation, used by the handle(_:forProperties:handler:) method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNParticleEventBlock = (UnsafeMutablePointer, UnsafeMutablePointer, UnsafeMutablePointer?, Int) -> Void
```

## Discussion

The block takes the following parameters:

data  
An array of floating-point values containing stripes of property data for the system’s particles. The width and format of each data stripe depend on the properties you specify when calling the handle(_:forProperties:handler:) method.

dataStride  
An array identifying the offset, in bytes, of each property’s value in the data stripe for each particle. The order of offsets in this array corresponds to the order of the `properties` array you specify when calling the handle(_:forProperties:handler:) method.

indices  
An array in which each element is an index that identifies (in the `data` array) the data stripe for each particle affected by the event that caused SceneKit to call the handler block.

When SceneKit calls your handler block for the SCNParticleEvent.birth event, you need not use this parameter—at that time, the affected particles are indexed from `0` to the `count` parameter’s value.

count  
The number of particles affected by the current event.

Use this block to change properties of individual particles when they are spawned, when they collide with scene geometry, or when they die (that is, reach the end of their life spans and are removed from the scene).

The following example illustrates setting up a handler block for particle collision events:

```
[system handleEvent:SCNParticleEventCollision
      forProperties:@[SCNParticlePropertyAngle,
                      SCNParticlePropertyRotationAxis,
                      SCNParticlePropertyContactNormal]
          withBlock:^(void **data, size_t *dataStride, uint32_t *indices, NSInteger count) {
              // For each particle affected by the collision event,
              // calculate pointers in the data to each property's value.
              for (NSInteger i = 0; i 

## See Also

### Modifying Particles in Response to Particle System Events

func handle(SCNParticleEvent, forProperties: [SCNParticleSystem.ParticleProperty], handler: SCNParticleEventBlock)

Adds a block that modifies particle properties, to be executed at a specified event in the lifetimes of particles in the system.

enum SCNParticleEvent

Significant events in the life spans of simulate particles, used by the handle(_:forProperties:handler:) method.

