

- SpriteKit
- SKEmitterNode
-  particleBlendMode 

Instance Property

# particleBlendMode

The blending mode used to blend particles into the framebuffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleBlendMode: SKBlendMode { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleBlendMode: SKBlendMode { get set }
```

## Discussion

The default value is SKBlendMode.alpha.

## See Also

### Blending Particles with the Framebuffer

var particleAlphaSequence: SKKeyframeSequence?

The sequence used to specify the alpha value of a particle over its lifetime.

var particleAlpha: CGFloat

The average starting alpha value for a particle.

var particleAlphaRange: CGFloat

The range of allowed random values for a particle’s starting alpha value.

var particleAlphaSpeed: CGFloat

The rate at which the alpha value of a particle changes per second.

