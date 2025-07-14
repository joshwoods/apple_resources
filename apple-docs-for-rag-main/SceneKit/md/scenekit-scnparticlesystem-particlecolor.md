

- SceneKit
- SCNParticleSystem
-  particleColor 

Instance Property

# particleColor

The color of newly spawned particles. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**macOS**

``` source
var particleColor: NSColor { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
var particleColor: UIColor { get set }
```

## Discussion

This color tints or shades the texture provided by the particleImage property. You can use this property to implement a range of many possible visual effects using the same artwork. For example, a small, blurry, white circle texture can be tinted yellow or orange to simulate fire, shaded gray or black to simulate smoke, or left alone to simulate falling snow.

The default color is white, causing the particle image to appear without tint or shading.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Specifying Particle Appearance

var particleSize: CGFloat

The rendered size, in units of the scene’s world coordinate space, of the particle image. Animatable.

var particleSizeVariation: CGFloat

The range of randomized particle sizes. Animatable.

var particleColorVariation: SCNVector4

The ranges of randomized particle color components. Animatable.

var particleImage: Any?

The texture image SceneKit uses to render each particle.

var fresnelExponent: CGFloat

The reflectivity exponent SceneKit uses when rendering the particle’s image as a cube map. Animatable.

var stretchFactor: CGFloat

A multiplier for stretching particle images along their direction of motion. Animatable.

