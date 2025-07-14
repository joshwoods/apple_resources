

- Model I/O
-  MDLTextureFilter 

Class

# MDLTextureFilter

A description of filtering modes for a renderer to use when sampling from a texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLTextureFilter
```

## Overview

A texture filter, together with a MDLTexture object and transform information, form a MDLTextureSampler object, which describes a texture and its rendering parameters for use in rendering one aspect of a MDLMaterial object’s surface appearance.

## Topics

### Managing Texture Coordinate Wrap Modes

var sWrapMode: MDLMaterialTextureWrapMode

The coordinate wrapping mode for texture t-coordinates.

var tWrapMode: MDLMaterialTextureWrapMode

The coordinate wrapping mode for texture t-coordinates.

var rWrapMode: MDLMaterialTextureWrapMode

The coordinate wrapping mode for texture r-coordinates.

### Managing Texture Filter Modes

var minFilter: MDLMaterialTextureFilterMode

The filter mode for rendering textures at sizes smaller than that of the original image.

var magFilter: MDLMaterialTextureFilterMode

The filter mode for rendering textures at sizes larger than that of the original image.

var mipFilter: MDLMaterialMipMapFilterMode

The filter mode for rendering textures using mipmapping.

### Constants

enum MDLMaterialTextureWrapMode

Modes for sampling textures at coordinates outside the texture bounds, used by the sWrapMode, tWrapMode, and rWrapMode properties.

enum MDLMaterialTextureFilterMode

Modes for sampling textures at coordinates between texels, used by the minFilter and magFilter properties.

enum MDLMaterialMipMapFilterMode

Modes for sampling textures at sizes between mipmap levels, used by the mipFilter property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Textures

class MDLTexture

A source of texel data to be used in rendering material surface appearances.

class MDLCheckerboardTexture

A generator of texel data that creates a checkerboard pattern with two specified colors.

class MDLColorSwatchTexture

A generator of texel data that creates a gradient between two specified colors.

class MDLNoiseTexture

A generator of texel data that creates a field of random noise.

class MDLNormalMapTexture

A generator of texel data that computes a normal map from a supplied texture.

class MDLSkyCubeTexture

A generator of texel data that creates cube textures using a physically realistic simulation of the sunlit sky.

class MDLURLTexture

A lightweight reference to a URL from which to load texture data.

class MDLTextureSampler

An object that pairs a source of texture data with sampling parameters to be used in rendering the texture.

