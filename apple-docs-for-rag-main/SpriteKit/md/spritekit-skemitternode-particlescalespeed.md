

- SpriteKit
- SKEmitterNode
-  particleScaleSpeed 

Instance Property

# particleScaleSpeed

The rate at which a particle’s scale factor changes per second.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleScaleSpeed: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleScaleSpeed: CGFloat { get set }
```

## Discussion

The default value is `0.0`.

## See Also

### Scaling Particles by a Factor

var particleScale: CGFloat

The average initial scale factor of a particle.

var particleScaleRange: CGFloat

The range of allowed random values for a particle’s initial scale.

var particleScaleSequence: SKKeyframeSequence?

The sequence used to specify the scale factor of a particle over its lifetime.

