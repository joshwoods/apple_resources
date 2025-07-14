

- SpriteKit
- SKEmitterNode
-  emissionAngleRange 

Instance Property

# emissionAngleRange

The range of allowed random values for a particle’s initial direction, expressed as an angle in radians.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var emissionAngleRange: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var emissionAngleRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the emission angle of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Controlling Particle Velocity and Acceleration

var particleSpeed: CGFloat

The average initial speed of a new particle, in points per second.

var particleSpeedRange: CGFloat

The range of allowed random values for a particle’s initial speed.

var emissionAngle: CGFloat

The average initial direction of a particle, expressed as an angle in radians.

var xAcceleration: CGFloat

The acceleration to apply to a particle’s horizontal velocity.

var yAcceleration: CGFloat

The acceleration to apply to a particle’s vertical velocity.

var particleZPositionSpeed: CGFloat

The speed at which the particle’s depth changes.

