

- SceneKit
- SCNMaterialProperty
-  maxAnisotropy 

Instance Property

# maxAnisotropy

The amount of anisotropic texture filtering to be used when rendering the material property’s image contents.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var maxAnisotropy: CGFloat { get set }
```

## Discussion

Anisotropic filtering is a process that increases the quality of texture rendering when a textured surface appears at an extreme angle relative to the camera. This process works by sampling from multiple mipmap levels of a texture for each rendered pixel—the term anisotropy refers to the number of samples per pixel. A higher anisotropy improves rendering quality, but at a cost to rendering performance.

For example, the image on the left in the figure below uses no anisotropic filtering, resulting in rendering artifacts as the checkerboard pattern recedes into the distance. The other images use higher maxAnisotropy values, reducing rendering artifacts. Anisotropic filtering requires mipmaps, so this property only takes effect if the value of the mipFilter property is not SCNFilterMode.none.

SceneKit automatically increases or decreases anisotropy for each rendered pixel as needed to maximize rendering quality, up to the limit specified by this property. The maximum anisotropy level used when rendering is dependent on the graphics hardware in use. Set this property’s value to the `MAXFLOAT` constant (the default) to use the highest anisotropy level supported by the GPU. A maxAnisotropy value of `1.0` or lower disables anisotropic filtering.

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

var mappingChannel: Int

The source of texture coordinates for mapping the material property’s image contents.

var borderColor: Any?

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

Deprecated

