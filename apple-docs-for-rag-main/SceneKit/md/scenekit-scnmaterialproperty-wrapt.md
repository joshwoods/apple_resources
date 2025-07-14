

- SceneKit
- SCNMaterialProperty
-  wrapT 

Instance Property

# wrapT

The wrapping behavior for the T texture coordinate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var wrapT: SCNWrapMode { get set }
```

## Discussion

Wrapping modes determine texture mapping behavior for cases where a material’s texture coordinates extend outside the range from `0.0` to `1.0`. For example, if you use the contentsTransform property to shrink a texture relative to the surface of a geometry, you use the wrap mode properties to determine whether the texture repeats across the surface.

The T texture coordinate measures the vertical axis of a texture image, increasing from `0.0` at the bottom of the image to `1.0` at the top.

The default wrap mode is SCNWrapMode.clamp. See SCNWrapMode for available modes and their effects.

## See Also

### Configuring Texture Mapping Attributes

var contentsTransform: SCNMatrix4

The transformation applied to the material property’s visual contents. Animatable.

var wrapS: SCNWrapMode

The wrapping behavior for the S texture coordinate.

enum SCNWrapMode

Modes to apply to texture wrapping, used by the wrapT and wrapS properties.

var minificationFilter: SCNFilterMode

Texture filtering for rendering the material property’s image contents at a size smaller than that of the original image.

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

