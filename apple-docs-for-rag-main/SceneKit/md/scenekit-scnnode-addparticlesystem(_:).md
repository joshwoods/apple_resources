

- SceneKit
- SCNNode
-  addParticleSystem(\_:) 

Instance Method

# addParticleSystem(\_:)

Attaches a particle system to the node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func addParticleSystem(_ system: SCNParticleSystem)
```

## Parameters 

`system`  

A particle system.

## Discussion

When attached to a node, a particle system’s emitter location follows that node as it moves through the scene. To instead attach a particle system to a location in the scene’s world coordinate space, use the corresponding method on SCNScene.

For details on particle systems, see SCNParticleSystem.

## See Also

### Working with Particle Systems

var particleSystems: [SCNParticleSystem]?

The particle systems attached to the node.

func removeParticleSystem(SCNParticleSystem)

Removes a particle system attached to the node.

func removeAllParticleSystems()

Removes any particle systems directly attached to the node.

