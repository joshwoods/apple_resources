

- SceneKit
- SCNScene
-  removeParticleSystem(\_:) 

Instance Method

# removeParticleSystem(\_:)

Removes a particle system attached to the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func removeParticleSystem(_ system: SCNParticleSystem)
```

## Parameters 

`system`  

A particle system.

## Discussion

This method has no effect if the `system` parameter does not reference a particle system directly attached to the scene.

## See Also

### Working with Particle Systems in the Scene

func addParticleSystem(SCNParticleSystem, transform: SCNMatrix4)

Attaches a particle system to the scene, using the specified transform.

var particleSystems: [SCNParticleSystem]?

The particle systems attached to the scene.

func removeAllParticleSystems()

Removes any particle systems directly attached to the scene.

