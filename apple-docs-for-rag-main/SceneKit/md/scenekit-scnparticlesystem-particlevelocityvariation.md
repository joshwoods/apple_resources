

- SceneKit
- SCNParticleSystem
-  particleVelocityVariation 

Instance Property

# particleVelocityVariation

The range, in units per second, of randomized initial particle speeds. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleVelocityVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the particleVelocity property. SceneKit randomly adjusts the initial speed of each particle by up to half the particleVelocityVariation value. For example, if the particleVelocity value is `10.0` units per second and the particleVelocityVariation value is `5.0` units per second, newly spawned particles have random velocities between `7.5` and `12.5` units per second.

The default value is `0.0` units per second, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Particle Motion

var particleAngle: CGFloat

The rotation angle, in degrees, of newly spawned particles. Animatable.

var particleAngleVariation: CGFloat

The range, in degrees of randomized initial particle angles. Animatable.

var particleVelocity: CGFloat

The initial speed, in units per second, for newly spawned particles. Animatable.

var particleAngularVelocity: CGFloat

The initial spin rate, in degrees per second, of newly spawned particles. Animatable.

var particleAngularVelocityVariation: CGFloat

The range, in degrees per second, of randomized initial angular velocities for particles. Animatable.

var particleLifeSpan: CGFloat

The duration, in seconds, for which each particle is rendered before being removed from the scene. Animatable.

var particleLifeSpanVariation: CGFloat

The range, in seconds, of randomized particle life spans. Animatable.

