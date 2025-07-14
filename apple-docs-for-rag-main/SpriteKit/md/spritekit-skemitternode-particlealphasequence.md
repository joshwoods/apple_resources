

- SpriteKit
- SKEmitterNode
-  particleAlphaSequence 

Instance Property

# particleAlphaSequence

The sequence used to specify the alpha value of a particle over its lifetime.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleAlphaSequence: SKKeyframeSequence? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleAlphaSequence: SKKeyframeSequence? { get set }
```

## Mentioned in 

Using Keyframe Sequence to effect Custom Interpolation

Animating Particle Properties Across Disparate Values

## Discussion

The default value is `nil`. If a non-`nil` value is specified, then the particleAlpha, particleAlphaRange, and particleAlphaSpeed properties are ignored. Instead, the sequence is used to specify the alpha value.

## See Also

### Blending Particles with the Framebuffer

var particleBlendMode: SKBlendMode

The blending mode used to blend particles into the framebuffer.

var particleAlpha: CGFloat

The average starting alpha value for a particle.

var particleAlphaRange: CGFloat

The range of allowed random values for a particle’s starting alpha value.

var particleAlphaSpeed: CGFloat

The rate at which the alpha value of a particle changes per second.

