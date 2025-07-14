

- SceneKit
- SCNParticleSystem
-  emissionDuration 

Instance Property

# emissionDuration

The duration, in seconds, over which the system spawns new particles. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var emissionDuration: CGFloat { get set }
```

## Discussion

The birthRate property determines the number of particles spawned during this duration. You can randomize the duration with the emissionDurationVariation property.

A duration of `0.0` specifies that all particles (the value of the birthRate property) spawn instantaneously. Use this duration to create randomized static effects in your scene. For example, by combining this option with the birthLocation and imageSequenceInitialFrameVariation properties, you can cover a plane with a variety of sprites, creating the appearance of a grassy field.

The default value is `1.0` seconds.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Particle Emission Timing

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

var birthRateVariation: CGFloat

The range of randomized particle birth rate values. Animatable.

