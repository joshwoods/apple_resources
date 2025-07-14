

- SpriteKit
- SKEmitterNode
-  particleColorBlendFactorSequence 

Instance Property

# particleColorBlendFactorSequence

The sequence used to specify the color blend factor of a particle over its lifetime.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleColorBlendFactorSequence: SKKeyframeSequence? { get set }
```

**watchOS**

``` source
var particleColorBlendFactorSequence: SKKeyframeSequence? { get set }
```

## Mentioned in 

Using Keyframe Sequence to effect Custom Interpolation

Animating Particle Properties Across Disparate Values

## Discussion

The default value is `nil`. If a non-`nil` value is specified, then the particleColorBlendFactor, particleColorBlendFactorRange, and particleColorBlendFactorSpeed properties are ignored. Instead, the sequence is used to specify the color blend factor.

## See Also

### Controlling How the Texture is Blended with Particle Color

var particleColorBlendFactor: CGFloat

The average starting value for the color blend factor.

var particleColorBlendFactorRange: CGFloat

The range of allowed random values for a particle’s starting color blend factor.

var particleColorBlendFactorSpeed: CGFloat

The rate at which the color blend factor changes per second.

