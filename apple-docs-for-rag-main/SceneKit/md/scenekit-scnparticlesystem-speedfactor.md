

- SceneKit
- SCNParticleSystem
-  speedFactor 

Instance Property

# speedFactor

A multiplier for the speed at which SceneKit runs the particle simulation. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var speedFactor: CGFloat { get set }
```

## Discussion

Use this property to speed up or slow down the overall behavior of a particle system without changing the many individual properties (such as acceleration, particleAngularVelocity, and particleBounce) that affect the motion of particles.

The default value is 1.0. Lower values slow down the effect; higher values make the effect run faster.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Controlling Particle Simulation

var isLocal: Bool

A Boolean value that specifies whether the particle simulation runs in the local coordinate space of the node containing it.

func reset()

Returns the particle system to its initial state.

