

- SceneKit
- SCNParticleSystem
-  particleImage 

Instance Property

# particleImage

The texture image SceneKit uses to render each particle.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var particleImage: Any? { get set }
```

## Discussion

Texture images help to determine visual effect rendered by the particle system. The particleColor property colorizes the image before rendering. You may specify an image using an NSImage (in macOS) or UIImage (in iOS) instance, or an NSString or NSURL instance containing the path or URL to an image file.

If the value is `nil` (the default), SceneKit renders each particle as a small white square (colorized by the particleColor property).

To specify a sequence of frames for animating each particle, arrange the frames as a grid in a single image, as shown in Figure 1, then use the properties listed in Animating Particle Images to identify frames in the grid and set the speed and style of the animation.

You can also create particles that appear reflective by assigning an array of images to this property. SceneKit treats the six images in the array as a cube map and renders each particle as a solid-color, reflective sphere. The particle system’s fresnelExponent property controls each sphere’s reflectivity. For details on cube map textures, see SCNMaterialProperty.

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

var fresnelExponent: CGFloat

The reflectivity exponent SceneKit uses when rendering the particle’s image as a cube map. Animatable.

var stretchFactor: CGFloat

A multiplier for stretching particle images along their direction of motion. Animatable.

