

- SceneKit
- SCNParticleSystem
-  particleVelocity 

Instance Property

# particleVelocity

The initial speed, in units per second, for newly spawned particles. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleVelocity: CGFloat { get set }
```

## Discussion

Particles begin moving at this speed in the direction determined by the birthDirection or emittingDirection property. Their directions and speeds may change thereafter according to the acceleration property or physics effects (see the isAffectedByGravity, isAffectedByPhysicsFields, and colliderNodes properties). You can randomize the speed of newly spawned particles with the particleAngularVelocityVariation property.

Particle speed is measured in units (of the local coordinate space containing the particle system) per second.

The default value is `0.0` units per second, specifying that newly emitted particles are stationary until otherwise influenced.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Particle Motion

var particleAngle: CGFloat

The rotation angle, in degrees, of newly spawned particles. Animatable.

var particleAngleVariation: CGFloat

The range, in degrees of randomized initial particle angles. Animatable.

var particleVelocityVariation: CGFloat

The range, in units per second, of randomized initial particle speeds. Animatable.

var particleAngularVelocity: CGFloat

The initial spin rate, in degrees per second, of newly spawned particles. Animatable.

var particleAngularVelocityVariation: CGFloat

The range, in degrees per second, of randomized initial angular velocities for particles. Animatable.

var particleLifeSpan: CGFloat

The duration, in seconds, for which each particle is rendered before being removed from the scene. Animatable.

var particleLifeSpanVariation: CGFloat

The range, in seconds, of randomized particle life spans. Animatable.

