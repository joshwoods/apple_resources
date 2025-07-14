

- SceneKit
- SCNParticleSystem
-  particleLifeSpan 

Instance Property

# particleLifeSpan

The duration, in seconds, for which each particle is rendered before being removed from the scene. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleLifeSpan: CGFloat { get set }
```

## Discussion

After each particle is spawned, it appears in the scene for a period of this duration before being removed from the scene. You can randomize the life spans of newly spawned particles with the particleLifeSpanVariation property.

The default value is `1.0` seconds.

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

var particleLifeSpanVariation: CGFloat

The range, in seconds, of randomized particle life spans. Animatable.

