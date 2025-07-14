

- SpriteKit
- SKEmitterNode
-  particleScaleRange 

Instance Property

# particleScaleRange

The range of allowed random values for a particle’s initial scale.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleScaleRange: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleScaleRange: CGFloat { get set }
```

## Discussion

The default value is `0.0`. If non-zero, the initial scale of each particle is randomly determined and may vary by plus or minus half of the range value.

## See Also

### Scaling Particles by a Factor

var particleScale: CGFloat

The average initial scale factor of a particle.

var particleScaleSpeed: CGFloat

The rate at which a particle’s scale factor changes per second.

var particleScaleSequence: SKKeyframeSequence?

The sequence used to specify the scale factor of a particle over its lifetime.

