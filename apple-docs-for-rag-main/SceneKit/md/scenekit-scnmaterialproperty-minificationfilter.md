

- SceneKit
- SCNMaterialProperty
-  minificationFilter 

Instance Property

# minificationFilter

Texture filtering for rendering the material property’s image contents at a size smaller than that of the original image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var minificationFilter: SCNFilterMode { get set }
```

## Discussion

Texture filtering determines the appearance of a material property’s contents when portions of the material surface appear larger or smaller than the original texture image. For example, the texture coordinates at a point far from the camera may correspond to an area of several pixels in the texture image. SceneKit uses the minification filter to determine the color of the sampled texel at that point.

The default minification filter is SCNFilterMode.linear. See SCNWrapMode for available modes and their effects.

## See Also

### Configuring Texture Mapping Attributes

var contentsTransform: SCNMatrix4

The transformation applied to the material property’s visual contents. Animatable.

var wrapS: SCNWrapMode

The wrapping behavior for the S texture coordinate.

var wrapT: SCNWrapMode

The wrapping behavior for the T texture coordinate.

enum SCNWrapMode

Modes to apply to texture wrapping, used by the wrapT and wrapS properties.

var magnificationFilter: SCNFilterMode

Texture filtering for rendering the material property’s image contents at a size larger than that of the original image.

var mipFilter: SCNFilterMode

Texture filtering for using mipmaps to render the material property’s image contents at a size smaller than that of the original image.

enum SCNFilterMode

Texture filtering modes, used by the minificationFilter, magnificationFilter, and mipFilter properties.

var maxAnisotropy: CGFloat

The amount of anisotropic texture filtering to be used when rendering the material property’s image contents.

var mappingChannel: Int

The source of texture coordinates for mapping the material property’s image contents.

var borderColor: Any?

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

Deprecated

