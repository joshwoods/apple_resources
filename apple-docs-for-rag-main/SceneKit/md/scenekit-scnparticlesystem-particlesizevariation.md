

- SceneKit
- SCNParticleSystem
-  particleSizeVariation 

Instance Property

# particleSizeVariation

The range of randomized particle sizes. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleSizeVariation: CGFloat { get set }
```

## Discussion

Setting a nonzero value for this property randomizes the effect of the particleSize property. SceneKit randomly adjusts the size of each particle by up to half the particleSizeVariation value. For example, if the particleSize value is `1.0` and the particleSizeVariation value is `0.5`, newly spawned particles are randomly sized between `0.75` and `1.25` units wide and high.

The default value is `0.0`, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Specifying Particle Appearance

var particleSize: CGFloat

The rendered size, in units of the scene’s world coordinate space, of the particle image. Animatable.

var particleColor: UIColor

The color of newly spawned particles. Animatable.

var particleColorVariation: SCNVector4

The ranges of randomized particle color components. Animatable.

var particleImage: Any?

The texture image SceneKit uses to render each particle.

var fresnelExponent: CGFloat

The reflectivity exponent SceneKit uses when rendering the particle’s image as a cube map. Animatable.

var stretchFactor: CGFloat

A multiplier for stretching particle images along their direction of motion. Animatable.

