

- SpriteKit
- SKEmitterNode
-  particleSpeedRange 

Instance Property

# particleSpeedRange

The range of allowed random values for a particle’s initial speed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleSpeedRange: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleSpeedRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the speed of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Controlling Particle Velocity and Acceleration

var particleSpeed: CGFloat

The average initial speed of a new particle, in points per second.

var emissionAngle: CGFloat

The average initial direction of a particle, expressed as an angle in radians.

var emissionAngleRange: CGFloat

The range of allowed random values for a particle’s initial direction, expressed as an angle in radians.

var xAcceleration: CGFloat

The acceleration to apply to a particle’s horizontal velocity.

var yAcceleration: CGFloat

The acceleration to apply to a particle’s vertical velocity.

var particleZPositionSpeed: CGFloat

The speed at which the particle’s depth changes.

