

- SpriteKit
- SKEmitterNode
-  particleColorBlendFactorRange 

Instance Property

# particleColorBlendFactorRange

The range of allowed random values for a particle’s starting color blend factor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleColorBlendFactorRange: CGFloat { get set }
```

**watchOS**

``` source
var particleColorBlendFactorRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the initial color blend factor of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Controlling How the Texture is Blended with Particle Color

var particleColorBlendFactorSequence: SKKeyframeSequence?

The sequence used to specify the color blend factor of a particle over its lifetime.

var particleColorBlendFactor: CGFloat

The average starting value for the color blend factor.

var particleColorBlendFactorSpeed: CGFloat

The rate at which the color blend factor changes per second.

