

- SceneKit
- SCNParticleSystem
-  birthRateVariation 

Instance Property

# birthRateVariation

The range of randomized particle birth rate values. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var birthRateVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the birthRate property. For each emission period, SceneKit randomly adjusts the birth rate by up to half the birthRateVariation value. For example, if the birthRate value is `100` particles and the birthRateVariation value is `50` particles, the system randomly emits between 75 and 125 particles during its emissionDuration period.

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

var idleDurationVariation: CGFloat

The range, in seconds, of randomized idle duration values. Animatable.

var loops: Bool

A Boolean value that determines whether the system repeats its emission and idle periods.

var warmupDuration: CGFloat

The duration, in seconds, for which particles are spawned before the system is first rendered. Animatable.

var birthRate: CGFloat

The number of particles spawned during each emission period. Animatable.

