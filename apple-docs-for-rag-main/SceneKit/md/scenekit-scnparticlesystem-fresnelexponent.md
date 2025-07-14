

- SceneKit
- SCNParticleSystem
-  fresnelExponent 

Instance Property

# fresnelExponent

The reflectivity exponent SceneKit uses when rendering the particle’s image as a cube map. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var fresnelExponent: CGFloat { get set }
```

## Discussion

This property only takes effect when the particleImage property is an array of six images defining a cube map. In this case, SceneKit renders each particle as a reflective sphere.

The *fresnel exponent* modulates the reflectivity of a surface from different view angles. At the default value of `1.0`, reflections have the same intensity across the entire surface of the particle. At higher values, the edges of the particle are more reflective than the center.

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

var stretchFactor: CGFloat

A multiplier for stretching particle images along their direction of motion. Animatable.

