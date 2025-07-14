

- SceneKit
- SCNParticleSystem
-  particleLifeSpanVariation 

Instance Property

# particleLifeSpanVariation

The range, in seconds, of randomized particle life spans. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleLifeSpanVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the particleLifeSpan property. SceneKit randomly adjusts the life span of each particle by up to half the particleLifeSpanVariation value. For example, if the particleLifeSpan value is `1.0` seconds and the particleLifeSpanVariation value is `0.5` seconds, each particle appears for a random duration between `0.75` and `1.25` seconds before being removed from the scene.

The default value is `0.0` seconds, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Particle Motion

var particleAngle: CGFloat

The rotation angle, in degrees, of newly spawned particles. Animatable.

var particleAngleVariation: CGFloat

The range, in degrees of randomized initial particle angles. Animatable.

var particleVelocity: CGFloat

The initial speed, in units per second, for newly spawned particles. Animatable.

var particleVelocityVariation: CGFloat

The range, in units per second, of randomized initial particle speeds. Animatable.

var particleAngularVelocity: CGFloat

The initial spin rate, in degrees per second, of newly spawned particles. Animatable.

var particleAngularVelocityVariation: CGFloat

The range, in degrees per second, of randomized initial angular velocities for particles. Animatable.

var particleLifeSpan: CGFloat

The duration, in seconds, for which each particle is rendered before being removed from the scene. Animatable.

