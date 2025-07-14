

- SpriteKit
- SKEmitterNode
-  particleAlpha 

Instance Property

# particleAlpha

The average starting alpha value for a particle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleAlpha: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleAlpha: CGFloat { get set }
```

## Discussion

The particle alpha value is equivalent to the alpha property of the SKNode class. The alpha component of the color that results from the texture and color blending state is multiplied by a particle’s alpha value. The resulting particle color is then blended with the parent’s framebuffer. The default value is `1.0`.

## See Also

### Blending Particles with the Framebuffer

var particleBlendMode: SKBlendMode

The blending mode used to blend particles into the framebuffer.

var particleAlphaSequence: SKKeyframeSequence?

The sequence used to specify the alpha value of a particle over its lifetime.

var particleAlphaRange: CGFloat

The range of allowed random values for a particle’s starting alpha value.

var particleAlphaSpeed: CGFloat

The rate at which the alpha value of a particle changes per second.

