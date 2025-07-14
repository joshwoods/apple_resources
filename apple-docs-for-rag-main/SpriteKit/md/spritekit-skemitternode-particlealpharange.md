

- SpriteKit
- SKEmitterNode
-  particleAlphaRange 

Instance Property

# particleAlphaRange

The range of allowed random values for a particle’s starting alpha value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleAlphaRange: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleAlphaRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the initial alpha value of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Blending Particles with the Framebuffer

var particleBlendMode: SKBlendMode

The blending mode used to blend particles into the framebuffer.

var particleAlphaSequence: SKKeyframeSequence?

The sequence used to specify the alpha value of a particle over its lifetime.

var particleAlpha: CGFloat

The average starting alpha value for a particle.

var particleAlphaSpeed: CGFloat

The rate at which the alpha value of a particle changes per second.

