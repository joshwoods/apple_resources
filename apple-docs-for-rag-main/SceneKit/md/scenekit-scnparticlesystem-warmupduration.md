

- SceneKit
- SCNParticleSystem
-  warmupDuration 

Instance Property

# warmupDuration

The duration, in seconds, for which particles are spawned before the system is first rendered. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var warmupDuration: CGFloat { get set }
```

## Discussion

The default value is `0.0` seconds, specifying that the system begins emitting particles on the first frame SceneKit renders it in. Change this value to “fast forward” the particle system so that it appears to have been running for some amount of time when it is first rendered.

For example, consider a particle system that simulates falling snow. With the default behavior, the scene is initially clear of snowflakes, which only begin to fall as the scene appears. If you set a warmupDuration duration of several seconds, the scene will be already filled with falling snow when it first appears.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Particle Emission Timing

var emissionDuration: CGFloat

The duration, in seconds, over which the system spawns new particles. Animatable.

var emissionDurationVariation: CGFloat

The range, in seconds, of randomized emission duration values. Animatable.

var idleDuration: CGFloat

The duration, in seconds, of periods when the system emits no particles. Animatable.

var idleDurationVariation: CGFloat

The range, in seconds, of randomized idle duration values. Animatable.

var loops: Bool

A Boolean value that determines whether the system repeats its emission and idle periods.

var birthRate: CGFloat

The number of particles spawned during each emission period. Animatable.

var birthRateVariation: CGFloat

The range of randomized particle birth rate values. Animatable.

