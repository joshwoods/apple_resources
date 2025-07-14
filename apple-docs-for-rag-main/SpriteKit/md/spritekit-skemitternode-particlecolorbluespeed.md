

- SpriteKit
- SKEmitterNode
-  particleColorBlueSpeed 

Instance Property

# particleColorBlueSpeed

The rate at which the blue component of a particle’s color changes per second.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleColorBlueSpeed: CGFloat { get set }
```

**watchOS**

``` source
var particleColorBlueSpeed: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

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

var particleColorGreenRange: CGFloat

The range of allowed random values for the green component of a particle’s initial color.

var particleColorRedRange: CGFloat

The range of allowed random values for the red component of a particle’s initial color.

var particleColorAlphaSpeed: CGFloat

The rate at which the alpha component of a particle’s color changes per second.

var particleColorGreenSpeed: CGFloat

The rate at which the green component of a particle’s color changes per second.

var particleColorRedSpeed: CGFloat

The rate at which the red component of a particle’s color changes per second.

