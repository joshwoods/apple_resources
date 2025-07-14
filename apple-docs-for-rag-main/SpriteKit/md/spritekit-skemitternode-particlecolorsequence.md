

- SpriteKit
- SKEmitterNode
-  particleColorSequence 

Instance Property

# particleColorSequence

The sequence used to specify the color components of a particle over its lifetime.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleColorSequence: SKKeyframeSequence? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleColorSequence: SKKeyframeSequence? { get set }
```

## Mentioned in 

Animating Particle Properties Across Disparate Values

Using Keyframe Sequence to effect Custom Interpolation

## Discussion

The default value is `nil`. If a non-`nil` value is specified, then the particleColor, particleColorAlphaRange, particleColorRedRange, particleColorGreenRange, particleColorBlueRange, particleColorAlphaSpeed, particleColorRedSpeed, particleColorGreenSpeed, and particleColorBlueSpeed properties are ignored. Instead, the sequence is used to specify the particle color.

Important

If you create an SKEmitterNode object using Xcode’s particle editor, it uses a color sequence to implement the color change.

## See Also

### Configuring Particle Color

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

var particleColorBlueSpeed: CGFloat

The rate at which the blue component of a particle’s color changes per second.

var particleColorGreenSpeed: CGFloat

The rate at which the green component of a particle’s color changes per second.

var particleColorRedSpeed: CGFloat

The rate at which the red component of a particle’s color changes per second.

