

- SpriteKit
- SKEmitterNode
-  particleColorGreenRange 

Instance Property

# particleColorGreenRange

The range of allowed random values for the green component of a particle’s initial color.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleColorGreenRange: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleColorGreenRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the starting green component of a particle’s color is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Configuring Particle Color

var particleColorSequence: SKKeyframeSequence?

The sequence used to specify the color components of a particle over its lifetime.

var particleColor: UIColor

The average initial color for a particle.

var particleColorAlphaRange: CGFloat

The range of allowed random values for the alpha component of a particle’s initial color.

var particleColorBlueRange: CGFloat

The range of allowed random values for the blue component of a particle’s initial color.

var particleColorRedRange: CGFloat

The range of allowed random values for the red component of a particle’s initial color.

var particleColorAlphaSpeed: CGFloat

The rate at which the alpha component of a particle’s color changes per second.

var particleColorBlueSpeed: CGFloat

The rate at which the blue component of a particle’s color changes per second.

var particleColorGreenSpeed: CGFloat

The rate at which the green component of a particle’s color changes per second.

var particleColorRedSpeed: CGFloat

The rate at which the red component of a particle’s color changes per second.

