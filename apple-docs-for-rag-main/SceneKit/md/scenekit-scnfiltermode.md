

- SceneKit
-  SCNFilterMode 

Enumeration

# SCNFilterMode

Texture filtering modes, used by the minificationFilter, magnificationFilter, and mipFilter properties.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
enum SCNFilterMode
```

## Overview

Texture filtering determines the appearance of a material property’s contents when portions of the material surface appear larger or smaller than the original texture image. For example, when a texture is applied to a plane that recedes away from the camera into the distance:

- The texture coordinates at a point near the camera may correspond to a small fraction of a pixel in the original image. SceneKit uses the magnificationFilter property to determine the color of the sampled texel at that point.

- The texture coordinates at a point far from the camera may correspond to an area of several pixels in the original image. SceneKit uses the minificationFilter property to determine the color of the sampled texel at that point.

SceneKit also uses the filter specified by the mipFilter property when generating mipmap levels for a texture image.

## Topics

### Constants

case none

No texture filtering is applied.

case nearest

Texture filtering returns the color from only one texel, whose location is nearest to the coordinates being sampled.

case linear

Texture filtering sample texels from the neighborhood of the coordinates being sampled and linearly interpolates their colors.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var maxAnisotropy: CGFloat

The amount of anisotropic texture filtering to be used when rendering the material property’s image contents.

var mappingChannel: Int

The source of texture coordinates for mapping the material property’s image contents.

var borderColor: Any?

A color used to fill in areas of a material’s surface not covered by the material property’s image contents.

Deprecated

