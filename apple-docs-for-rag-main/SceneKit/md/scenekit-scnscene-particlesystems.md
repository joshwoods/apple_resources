

- SceneKit
- SCNScene
-  particleSystems 

Instance Property

# particleSystems

The particle systems attached to the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleSystems: [SCNParticleSystem]? { get }
```

## Discussion

An array of SCNParticleSystem objects directly attached to the scene. This array does not include particle systems attached to nodes within the scene.

For details on particle systems, see SCNParticleSystem.

## See Also

### Working with Particle Systems in the Scene

func addParticleSystem(SCNParticleSystem, transform: SCNMatrix4)

Attaches a particle system to the scene, using the specified transform.

func removeParticleSystem(SCNParticleSystem)

Removes a particle system attached to the scene.

func removeAllParticleSystems()

Removes any particle systems directly attached to the scene.

