

- SceneKit
- SCNScene
-  addParticleSystem(\_:transform:) 

Instance Method

# addParticleSystem(\_:transform:)

Attaches a particle system to the scene, using the specified transform.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**macOS**

``` source
func addParticleSystem(
    _ system: SCNParticleSystem,
    transform: SCNMatrix4
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func addParticleSystem(
    _ system: SCNParticleSystem,
    transform: SCNMatrix4
)
```

## Parameters 

`system`  

A particle system.

`transform`  

A transformation matrix that positions and orients the particle system relative to the world coordinate space of the scene.

## Discussion

A particle system directly attached to a scene is not related to the coordinate space of any node in the scene. To attach a particle system whose emitter location follows the movement of a node within the scene, use the corresponding SCNNode method.

For details on particle systems, see SCNParticleSystem.

## See Also

### Working with Particle Systems in the Scene

var particleSystems: [SCNParticleSystem]?

The particle systems attached to the scene.

func removeParticleSystem(SCNParticleSystem)

Removes a particle system attached to the scene.

func removeAllParticleSystems()

Removes any particle systems directly attached to the scene.

