

- SceneKit
- SCNMaterialProperty
-  borderColor Deprecated

Instance Property

# borderColor

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedmacOS 10.8–10.12Deprecated

``` source
var borderColor: Any? { get set }
```

Deprecated

Deprecated

## Discussion

When the material property’s contents are a texture image and its texture wrapping properties are set to SCNWrapMode.clampToBorder, the border color appears in areas of a textured geometry not covered by the texture image, as shown in .

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

