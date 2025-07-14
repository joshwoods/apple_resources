

- SpriteKit
- SKEmitterNode
-  particleScale 

Instance Property

# particleScale

The average initial scale factor of a particle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleScale: CGFloat { get set }
```

**watchOS**

``` source
var particleScale: CGFloat { get set }
```

## Discussion

The default value is `1.0`.

## See Also

### Scaling Particles by a Factor

var particleScaleRange: CGFloat

The range of allowed random values for a particle’s initial scale.

var particleScaleSpeed: CGFloat

The rate at which a particle’s scale factor changes per second.

var particleScaleSequence: SKKeyframeSequence?

The sequence used to specify the scale factor of a particle over its lifetime.

