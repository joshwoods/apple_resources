

- SceneKit
- SCNParticleSystem
-  idleDurationVariation 

Instance Property

# idleDurationVariation

The range, in seconds, of randomized idle duration values. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var idleDurationVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the idleDuration property. For each idle period, SceneKit randomly adjusts the duration by up to half the idleDurationVariation value. For example, if the idleDuration value is `1.0` seconds and the idleDurationVariation value is `0.5` seconds, the system idles for a period of `0.75` to `1.25` seconds between emissions.

The default value is `0.0` seconds, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Particle Emission Timing

var emissionDuration: CGFloat

The duration, in seconds, over which the system spawns new particles. Animatable.

var emissionDurationVariation: CGFloat

The range, in seconds, of randomized emission duration values. Animatable.

var idleDuration: CGFloat

The duration, in seconds, of periods when the system emits no particles. Animatable.

var loops: Bool

A Boolean value that determines whether the system repeats its emission and idle periods.

var warmupDuration: CGFloat

The duration, in seconds, for which particles are spawned before the system is first rendered. Animatable.

var birthRate: CGFloat

The number of particles spawned during each emission period. Animatable.

var birthRateVariation: CGFloat

The range of randomized particle birth rate values. Animatable.

