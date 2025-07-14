

- SpriteKit
- SKEmitterNode
-  particleZPositionSpeed 

Instance Property

# particleZPositionSpeed

The speed at which the particle’s depth changes.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedtvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleZPositionSpeed: CGFloat { get set }
```

**watchOS**

``` source
var particleZPositionSpeed: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Controlling Particle Velocity and Acceleration

var particleSpeed: CGFloat

The average initial speed of a new particle, in points per second.

var particleSpeedRange: CGFloat

The range of allowed random values for a particle’s initial speed.

var emissionAngle: CGFloat

The average initial direction of a particle, expressed as an angle in radians.

var emissionAngleRange: CGFloat

The range of allowed random values for a particle’s initial direction, expressed as an angle in radians.

var xAcceleration: CGFloat

The acceleration to apply to a particle’s horizontal velocity.

var yAcceleration: CGFloat

The acceleration to apply to a particle’s vertical velocity.

