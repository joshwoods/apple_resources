

- SceneKit
- SCNNode
-  particleSystems 

Instance Property

# particleSystems

The particle systems attached to the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleSystems: [SCNParticleSystem]? { get }
```

## Discussion

An array of SCNParticleSystem objects directly attached to the node. This array does not include particle systems attached to the node’s child nodes.

For details on particle systems, see SCNParticleSystem.

## See Also

### Working with Particle Systems

func addParticleSystem(SCNParticleSystem)

Attaches a particle system to the node.

func removeParticleSystem(SCNParticleSystem)

Removes a particle system attached to the node.

func removeAllParticleSystems()

Removes any particle systems directly attached to the node.

