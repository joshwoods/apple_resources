

- SceneKit
- SCNParticleSystem
-  reset() 

Instance Method

# reset()

Returns the particle system to its initial state.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func reset()
```

## Discussion

Calling this method removes all currently live particles from the scene.

## See Also

### Controlling Particle Simulation

var isLocal: Bool

A Boolean value that specifies whether the particle simulation runs in the local coordinate space of the node containing it.

var speedFactor: CGFloat

A multiplier for the speed at which SceneKit runs the particle simulation. Animatable.

