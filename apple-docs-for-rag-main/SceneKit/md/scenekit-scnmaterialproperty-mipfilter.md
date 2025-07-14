

- SceneKit
- SCNMaterialProperty
-  mipFilter 

Instance Property

# mipFilter

Texture filtering for using mipmaps to render the material property’s image contents at a size smaller than that of the original image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var mipFilter: SCNFilterMode { get set }
```

## Discussion

Mipmapping is a technique that can increase rendering performance when rendering a texture image at smaller sizes. SceneKit automatically creates several mipmap levels for the material property’s image contents, each at a fraction of the original image’s size. When rendering, SceneKit automatically samples texels from the mipmap level closest to the size being rendered.

If the value of this property is SCNFilterMode.none, SceneKit does not use mipmapping. If the value of this property is SCNFilterMode.linear, SceneKit determines pixel colors using trilinear filtering. First it linearly interpolates a texel color from each of the two mipmap levels closest to the target size, then it linearly interpolates between the two results to determine the final color. This technique provides higher rendering quality at moderate performance cost.

In iOS 10, tvOS 10, watchOS 3, and macOS 10.12, the default mipmapping filter mode is SCNFilterMode.nearest. In earlier OS versions, the default mode is SCNFilterMode.none.

The figure below shows the effects of enabling mipmapping. In the image on the left, mipmapping is disabled, causing pixelated artifacts as the checkerboard pattern recedes into the distance. Enabling linear mipmapping results in a smoother appearance.

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

enum SCNFilterMode

Texture filtering modes, used by the minificationFilter, magnificationFilter, and mipFilter properties.

var maxAnisotropy: CGFloat

The amount of anisotropic texture filtering to be used when rendering the material property’s image contents.

var mappingChannel: Int

The source of texture coordinates for mapping the material property’s image contents.

var borderColor: Any?

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

Deprecated

