

- SceneKit
- SCNParticleSystem
-  particleAngularVelocity 

Instance Property

# particleAngularVelocity

The initial spin rate, in degrees per second, of newly spawned particles. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleAngularVelocity: CGFloat { get set }
```

## Discussion

A particle’s angle (or orientation) is independent from its direction of motion. For example, a smoke effect may use a small image of a cloud for each particle, which stays at the same angle as the smoke rises, but a snow effect may use an image that flips and rotates as each snowflake falls. The orientationMode property determines whether and how particles are allowed to rotate, and the particleAngle and particleAngularVelocity properties determine rotation angles and rates. You can randomize the rotations of newly spawned particles with the particleAngleVariation property.

The default value is `0.0` degrees per second, specifying no rotation.

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

var particleAngularVelocityVariation: CGFloat

The range, in degrees per second, of randomized initial angular velocities for particles. Animatable.

var particleLifeSpan: CGFloat

The duration, in seconds, for which each particle is rendered before being removed from the scene. Animatable.

var particleLifeSpanVariation: CGFloat

The range, in seconds, of randomized particle life spans. Animatable.

