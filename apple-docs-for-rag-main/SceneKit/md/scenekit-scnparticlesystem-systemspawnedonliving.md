

- SceneKit
- SCNParticleSystem
-  systemSpawnedOnLiving 

Instance Property

# systemSpawnedOnLiving

Another particle system to be added to the scene for each living particle in the system.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var systemSpawnedOnLiving: SCNParticleSystem? { get set }
```

## Discussion

Each time SceneKit renders a frame, it adds an instance of the specified particle system to the scene at the location of each rendered particle.

Use this property to simulate continuous secondary effects on particles. For example, to create a fountain of sparklers, use one particle system as the fountain, and attach another system that simulates each sparkler.

The default value of this property is `nil`, specifying that no additional systems are added to the scene when rendering particles.

Important

This property adds one new particle system to the scene *for each rendered particle, on each rendered frame*, drastically increasing the total number of rendered particles. To avoid performance problems, plan your use of this property to limit the total number of particles in the scene. For example, attach a short-lived particle system to a system with few particles and whose loops property is set to false.

## See Also

### Spawning Additional Particle Systems

var systemSpawnedOnCollision: SCNParticleSystem?

Another particle system to be added to the scene when a particle collides with scene geometry.

var systemSpawnedOnDying: SCNParticleSystem?

Another particle system to be added to the scene when a particle dies.

