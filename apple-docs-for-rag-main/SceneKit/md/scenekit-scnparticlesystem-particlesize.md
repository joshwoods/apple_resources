

- SceneKit
- SCNParticleSystem
-  particleSize 

Instance Property

# particleSize

The rendered size, in units of the scene’s world coordinate space, of the particle image. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleSize: CGFloat { get set }
```

## Discussion

SceneKit uses this value for both the width and height of the particleImage texture at render time. (If you use the stretchFactor property to stretch particles in their direction of motion, the particleSize value determines the width and height before stretching.) You can randomize the sizes of newly spawned particles with the particleSizeVariation property.

The default value is `1.0`, specifying that particle images appear one unit high and one unit wide in the scene’s world coordinate space.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Specifying Particle Appearance

var particleSizeVariation: CGFloat

The range of randomized particle sizes. Animatable.

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

