

- SceneKit
- SCNParticleSystem
-  particleColorVariation 

Instance Property

# particleColorVariation

The ranges of randomized particle color components. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleColorVariation: SCNVector4 { get set }
```

## Discussion

This vector randomizes the color specified by the particleColor property. The components of the vector specify ranges of variation in hue, saturation, brightness, and alpha, in that order.

For example, consider the effects of different particleColorVariation vectors on a system whose particleColor property specifies a fully opaque red as the base color:

- The vector `{0.25, 0.0, 0.0, 0.0}` allows newly spawned particles to take on any hue within a quarter of the color wheel centered on red (that is, ranging from purple through magenta, red, orange, and yellow to green). Particles retain full saturation, brightness, and alpha.

- The vector `{0.0, 0.0, 0.0, 1.0}` allows newly spawned particles to vary in alpha between full and half opacity. (The range of variation is centered on the base value, but clamped to a maximum of `1.0`.) Particles retain the same hue, saturation, and brightness as the base color.

- The vector `{0.0, 1.0, 1.0, 0.0}` allows newly spawned particles to vary in saturation and brightness, resulting in random shades of red. Particles retain the same hue and alpha as the base color.

The default value is SCNVector4Zero, specifying no randomization.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Specifying Particle Appearance

var particleSize: CGFloat

The rendered size, in units of the scene’s world coordinate space, of the particle image. Animatable.

var particleSizeVariation: CGFloat

The range of randomized particle sizes. Animatable.

var particleColor: UIColor

The color of newly spawned particles. Animatable.

var particleImage: Any?

The texture image SceneKit uses to render each particle.

var fresnelExponent: CGFloat

The reflectivity exponent SceneKit uses when rendering the particle’s image as a cube map. Animatable.

var stretchFactor: CGFloat

A multiplier for stretching particle images along their direction of motion. Animatable.

