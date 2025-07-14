

- SceneKit
- SCNParticleSystem
-  systemSpawnedOnCollision 

Instance Property

# systemSpawnedOnCollision

Another particle system to be added to the scene when a particle collides with scene geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var systemSpawnedOnCollision: SCNParticleSystem? { get set }
```

## Discussion

When a particle collides with scene geometry, SceneKit adds a copy of the specified particle system to the scene at the location of the collision. (To define collision behavior, see the colliderNodes property.)

Use this property to simulate effects such as rain—one particle system simulates falling raindrops, and another particle system simulates the splashes that occur where each raindrop strikes a surface.

The default value of this property is `nil`, specifying that no additional systems are added to the scene on particle collision.

Important

Adding a new particle system to the scene for each collision can drastically increase the total number of rendered particles. To maintain adequate rendering performance, set the loops property to false for any particle system you assign to the systemSpawnedOnCollision property.

## See Also

### Spawning Additional Particle Systems

var systemSpawnedOnDying: SCNParticleSystem?

Another particle system to be added to the scene when a particle dies.

var systemSpawnedOnLiving: SCNParticleSystem?

Another particle system to be added to the scene for each living particle in the system.

