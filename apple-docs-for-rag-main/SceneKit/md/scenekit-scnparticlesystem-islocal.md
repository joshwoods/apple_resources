

- SceneKit
- SCNParticleSystem
-  isLocal 

Instance Property

# isLocal

A Boolean value that specifies whether the particle simulation runs in the local coordinate space of the node containing it.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isLocal: Bool { get set }
```

## Discussion

If false (the default), all positions, distances, and velocities in the particle system are in the scene’s world coordinate system. If true, the particle system runs in the local coordinate space of the node containing it.

Use this property to choose whether particles spawned by a moving emitter follow the system as it moves.

## See Also

### Controlling Particle Simulation

func reset()

Returns the particle system to its initial state.

var speedFactor: CGFloat

A multiplier for the speed at which SceneKit runs the particle simulation. Animatable.

