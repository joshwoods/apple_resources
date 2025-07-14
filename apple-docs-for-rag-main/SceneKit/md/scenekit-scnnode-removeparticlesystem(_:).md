

- SceneKit
- SCNNode
-  removeParticleSystem(\_:) 

Instance Method

# removeParticleSystem(\_:)

Removes a particle system attached to the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func removeParticleSystem(_ system: SCNParticleSystem)
```

## Parameters 

`system`  

A particle system.

## Discussion

This method has no effect if the `system` parameter does not reference a particle system directly attached to the node.

## See Also

### Working with Particle Systems

func addParticleSystem(SCNParticleSystem)

Attaches a particle system to the node.

var particleSystems: [SCNParticleSystem]?

The particle systems attached to the node.

func removeAllParticleSystems()

Removes any particle systems directly attached to the node.

