

- SpriteKit
- SKEmitterNode
-  particleAlphaSpeed 

Instance Property

# particleAlphaSpeed

The rate at which the alpha value of a particle changes per second.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleAlphaSpeed: CGFloat { get set }
```

**watchOS**

``` source
var particleAlphaSpeed: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Blending Particles with the Framebuffer

var particleBlendMode: SKBlendMode

The blending mode used to blend particles into the framebuffer.

var particleAlphaSequence: SKKeyframeSequence?

The sequence used to specify the alpha value of a particle over its lifetime.

var particleAlpha: CGFloat

The average starting alpha value for a particle.

var particleAlphaRange: CGFloat

The range of allowed random values for a particle’s starting alpha value.

