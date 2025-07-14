

- SceneKit
- SCNParticleSystem
-  stretchFactor 

Instance Property

# stretchFactor

A multiplier for stretching particle images along their direction of motion. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var stretchFactor: CGFloat { get set }
```

## Discussion

Use this property to create visual effects that show streaks of motion, such as fireworks. If the orientationMode property value is SCNParticleOrientationMode.free, a non-default stretch factor stretches particle images in the y-axis direction of each particle’s local coordinate space.

The default value is `0.0`, specifying that particle images maintain their original aspect ratio.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Specifying Particle Appearance

var particleSize: CGFloat

The rendered size, in units of the scene’s world coordinate space, of the particle image. Animatable.

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

