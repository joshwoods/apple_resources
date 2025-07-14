

- SpriteKit
- SKEmitterNode
-  particleColor 

Instance Property

# particleColor

The average initial color for a particle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var particleColor: UIColor { get set }
```

**macOS**

``` source
@MainActor
var particleColor: NSColor { get set }
```

**watchOS**

``` source
var particleColor: UIColor { get set }
```

## Discussion

The default value is `[SKColor clearColor]`.

A particle’s color is blended with the texture using its blend color factor. See SKEmitterNode.

Important

If you create an SKEmitterNode object using Xcode’s particle editor, it uses the particleColorSequence property to implement the color change. This means that the particleColor property is ignored.

## See Also

### Configuring Particle Color

var particleColorSequence: SKKeyframeSequence?

The sequence used to specify the color components of a particle over its lifetime.

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

var particleColorBlueSpeed: CGFloat

The rate at which the blue component of a particle’s color changes per second.

var particleColorGreenSpeed: CGFloat

The rate at which the green component of a particle’s color changes per second.

var particleColorRedSpeed: CGFloat

The rate at which the red component of a particle’s color changes per second.

