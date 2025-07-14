

- SpriteKit
- SKEmitterNode
-  particleZPosition 

Instance Property

# particleZPosition

The average starting depth of a particle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleZPosition: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleZPosition: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Controlling Particle Position

var particlePosition: CGPoint

The average starting position for a particle.

var particlePositionRange: CGVector

The range of allowed random values for a particle’s position.

var particleZPositionRange: CGFloat

The range of allowed random values for a particle’s depth.

