

- SpriteKit
- SKEmitterNode
-  particleScaleSequence 

Instance Property

# particleScaleSequence

The sequence used to specify the scale factor of a particle over its lifetime.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleScaleSequence: SKKeyframeSequence? { get set }
```

**watchOS**

``` source
var particleScaleSequence: SKKeyframeSequence? { get set }
```

## Mentioned in 

Animating Particle Properties Across Disparate Values

Using Keyframe Sequence to effect Custom Interpolation

## Discussion

The default value is `nil`. If a non-`nil` value is specified, then the particleScale, particleScaleRange, and particleScaleSpeed properties are ignored. Instead, the sequence is used to specify the scale factor.

## See Also

### Scaling Particles by a Factor

var particleScale: CGFloat

The average initial scale factor of a particle.

var particleScaleRange: CGFloat

The range of allowed random values for a particle’s initial scale.

var particleScaleSpeed: CGFloat

The rate at which a particle’s scale factor changes per second.

