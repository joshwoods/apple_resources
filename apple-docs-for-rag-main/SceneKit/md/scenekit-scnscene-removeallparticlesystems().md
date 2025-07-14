

- SceneKit
- SCNScene
-  removeAllParticleSystems() 

Instance Method

# removeAllParticleSystems()

Removes any particle systems directly attached to the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func removeAllParticleSystems()
```

## Discussion

Calling this method does not remove particle systems attached to nodes within the scene.

## See Also

### Working with Particle Systems in the Scene

func addParticleSystem(SCNParticleSystem, transform: SCNMatrix4)

Attaches a particle system to the scene, using the specified transform.

var particleSystems: [SCNParticleSystem]?

The particle systems attached to the scene.

func removeParticleSystem(SCNParticleSystem)

Removes a particle system attached to the scene.

