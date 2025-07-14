

- SpriteKit
- SKEmitterNode
-  particleColorBlendFactorSpeed 

Instance Property

# particleColorBlendFactorSpeed

The rate at which the color blend factor changes per second.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleColorBlendFactorSpeed: CGFloat { get set }
```

**watchOS**

``` source
var particleColorBlendFactorSpeed: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Controlling How the Texture is Blended with Particle Color

var particleColorBlendFactorSequence: SKKeyframeSequence?

The sequence used to specify the color blend factor of a particle over its lifetime.

var particleColorBlendFactor: CGFloat

The average starting value for the color blend factor.

var particleColorBlendFactorRange: CGFloat

The range of allowed random values for a particle’s starting color blend factor.

