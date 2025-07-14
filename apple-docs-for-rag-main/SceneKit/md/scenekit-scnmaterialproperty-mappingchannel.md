

- SceneKit
- SCNMaterialProperty
-  mappingChannel 

Instance Property

# mappingChannel

The source of texture coordinates for mapping the material property’s image contents.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var mappingChannel: Int { get set }
```

## Discussion

A geometry can have multiple independent sources of texture coordinates, each of which defines a unique mapping channel number. You can use these channels to map different visual properties of a material in different ways. For example, a geometry representing a picture frame might use one set of texture coordinates for mapping the materials of the frame itself, and another set of texture coordinates for placing a picture into the frame.

For information about creating geometries with multiple texture mapping channels, see SCNGeometry.

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

var borderColor: Any?

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

Deprecated

