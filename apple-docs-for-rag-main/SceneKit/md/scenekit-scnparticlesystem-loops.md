

- SceneKit
- SCNParticleSystem
-  loops 

Instance Property

# loops

A Boolean value that determines whether the system repeats its emission and idle periods.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var loops: Bool { get set }
```

## Discussion

If this value is true (the default), you can make the system emit particles periodically or sporadically. For example, in a looping system where the emissionDuration value is `1.0` seconds and the idleDuration value is `1.0` seconds, the system alternates alternates between equal one-second periods of spawning and not spawning particles. Use the emissionDurationVariation and idleDurationVariation properties to randomize the duration of each emission and idle period, making the emission behavior more sporadic.

Specify false for particle systems that create one-shot effects, such as an explosion that appears when a game character is defeated.

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

var warmupDuration: CGFloat

The duration, in seconds, for which particles are spawned before the system is first rendered. Animatable.

var birthRate: CGFloat

The number of particles spawned during each emission period. Animatable.

var birthRateVariation: CGFloat

The range of randomized particle birth rate values. Animatable.

