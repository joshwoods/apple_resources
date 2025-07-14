

- SceneKit
- SCNMaterialProperty
-  contentsTransform 

Instance Property

# contentsTransform

The transformation applied to the material property’s visual contents. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
var contentsTransform: SCNMatrix4 { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
var contentsTransform: SCNMatrix4 { get set }
```

## Discussion

SceneKit applies this transformation to the texture coordinates provided by the geometry object the material is attached to, then uses the resulting coordinates to map the material property’s contents across the surface of the material. (This transformation has no effect if the material property’s contents object is a constant color.)

For example, you can use this property to grow, offset, or rotate a texture relative to the surface of a material, as illustrated below.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Configuring Texture Mapping Attributes

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

var borderColor: Any?

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

Deprecated

