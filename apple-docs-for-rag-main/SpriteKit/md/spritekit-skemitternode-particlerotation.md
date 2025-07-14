

- SpriteKit
- SKEmitterNode
-  particleRotation 

Instance Property

# particleRotation

The average initial rotation of a particle, expressed as an angle in radians.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleRotation: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleRotation: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Adjusting a Particle’s Rotation

var particleRotationRange: CGFloat

The range of allowed random values for a particle’s initial rotation, expressed as an angle in radians.

var particleRotationSpeed: CGFloat

The speed at which a particle rotates, expressed in radians per second.

