

- SpriteKit
- SKEmitterNode
-  particleColorBlendFactor 

Instance Property

# particleColorBlendFactor

The average starting value for the color blend factor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleColorBlendFactor: CGFloat { get set }
```

**watchOS**

``` source
var particleColorBlendFactor: CGFloat { get set }
```

## Discussion

The default value is `0.0`, which means that the texture is used as is, ignoring the particle’s color. Otherwise, the texture is blended with the color. The maximum value is `1.0`, which means the particle renders with a full-tint color.

## See Also

### Controlling How the Texture is Blended with Particle Color

var particleColorBlendFactorSequence: SKKeyframeSequence?

The sequence used to specify the color blend factor of a particle over its lifetime.

var particleColorBlendFactorRange: CGFloat

The range of allowed random values for a particle’s starting color blend factor.

var particleColorBlendFactorSpeed: CGFloat

The rate at which the color blend factor changes per second.

