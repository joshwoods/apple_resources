

- SpriteKit
- SKEmitterNode
-  particlePosition 

Instance Property

# particlePosition

The average starting position for a particle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particlePosition: CGPoint { get set }
```

**watchOS**

``` source
var particlePosition: CGPoint { get set }
```

## Discussion

The default value is `(0.0,0.0)`.

## See Also

### Controlling Particle Position

var particlePositionRange: CGVector

The range of allowed random values for a particle’s position.

var particleZPosition: CGFloat

The average starting depth of a particle.

var particleZPositionRange: CGFloat

The range of allowed random values for a particle’s depth.

