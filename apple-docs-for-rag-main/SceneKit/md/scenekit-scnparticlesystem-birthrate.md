

- SceneKit
- SCNParticleSystem
-  birthRate 

Instance Property

# birthRate

The number of particles spawned during each emission period. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var birthRate: CGFloat { get set }
```

## Discussion

The system emits this number of particles at a constant rate through the duration of the period specified by the emissionDuration property. A value of zero prevents the system from emitting particles, unless you randomize the birth rate with the birthRateVariation property.

The default value is `1`.

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

var birthRateVariation: CGFloat

The range of randomized particle birth rate values. Animatable.

