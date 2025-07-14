

- SpriteKit
- SKEmitterNode
-  particlePositionRange 

Instance Property

# particlePositionRange

The range of allowed random values for a particle’s position.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particlePositionRange: CGVector { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particlePositionRange: CGVector { get set }
```

## Discussion

The default value is `(0.0,0.0)`. If a component is non-zero, the same component of a particle’s position is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Controlling Particle Position

var particlePosition: CGPoint

The average starting position for a particle.

var particleZPosition: CGFloat

The average starting depth of a particle.

var particleZPositionRange: CGFloat

The range of allowed random values for a particle’s depth.

