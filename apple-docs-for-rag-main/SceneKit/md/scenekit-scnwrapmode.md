

- SceneKit
-  SCNWrapMode 

Enumeration

# SCNWrapMode

Modes to apply to texture wrapping, used by the wrapT and wrapS properties.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
enum SCNWrapMode
```

## Overview

Wrapping modes determine texture mapping behavior for cases where a material’s texture coordinates extend outside the range from `0.0` to `1.0`. For example, if you use the contentsTransform property to shrink a texture relative to the surface of a geometry, you use the wrap mode properties to determine whether the texture repeats across the surface. The figure below shows the effect of each wrapping mode on an otherwise identical material.

## Topics

### Constants

case clamp

Texture coordinates are clamped to the range from `0.0` to `1.0`, inclusive.

case `repeat`

Texture sampling uses only the fractional part of texture coordinates, passing through the range from `0.0` to (but not including) `1.0`.

case clampToBorder

Texture sampling uses texture colors for coordinates in the range from `0.0` to `1.0` (inclusive) and the material property’s borderColor value otherwise.

case mirror

Texture sampling of texture coordinates outside range from `0.0` to `1.0` should behave as if the range reverses before repeating.

SCNClamp

Equivalent to SCNWrapMode.clamp.

SCNRepeat

Equivalent to SCNWrapMode.repeat.

SCNClampToBorder

Equivalent to SCNWrapMode.clampToBorder.

SCNMirror

Equivalent to SCNWrapMode.mirror.

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

