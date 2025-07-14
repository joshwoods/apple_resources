

- SceneKit
- SCNParticleSystem
-  idleDuration 

Instance Property

# idleDuration

The duration, in seconds, of periods when the system emits no particles. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var idleDuration: CGFloat { get set }
```

## Discussion

If the system’s loops property value is true, you can make the system emit particles periodically or sporadically. For example, in a looping system where the emissionDuration value is `1.0` seconds and the idleDuration value is `1.0` seconds, the system alternates between equal one-second periods of spawning and not spawning particles. You can randomize the duration with the idleDurationVariation property. Idle duration has no effect if the loops property value is false.

The default value is `0.0` seconds, specifying no idle time between emissions. (That is, if the loops property value is true, the system emits particles continuously.)

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Particle Emission Timing

var emissionDuration: CGFloat

The duration, in seconds, over which the system spawns new particles. Animatable.

var emissionDurationVariation: CGFloat

The range, in seconds, of randomized emission duration values. Animatable.

var idleDurationVariation: CGFloat

The range, in seconds, of randomized idle duration values. Animatable.

var loops: Bool

A Boolean value that determines whether the system repeats its emission and idle periods.

var warmupDuration: CGFloat

The duration, in seconds, for which particles are spawned before the system is first rendered. Animatable.

var birthRate: CGFloat

The number of particles spawned during each emission period. Animatable.

var birthRateVariation: CGFloat

The range of randomized particle birth rate values. Animatable.

