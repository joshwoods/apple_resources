

- SpriteKit
- SKEmitterNode
-  particleRotationRange 

Instance Property

# particleRotationRange

The range of allowed random values for a particle’s initial rotation, expressed as an angle in radians.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleRotationRange: CGFloat { get set }
```

**watchOS**

``` source
var particleRotationRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the initial rotation of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Adjusting a Particle’s Rotation

var particleRotation: CGFloat

The average initial rotation of a particle, expressed as an angle in radians.

var particleRotationSpeed: CGFloat

The speed at which a particle rotates, expressed in radians per second.

