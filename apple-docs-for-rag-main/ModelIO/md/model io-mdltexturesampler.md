

- Model I/O
-  MDLTextureSampler 

Class

# MDLTextureSampler

An object that pairs a source of texture data with sampling parameters to be used in rendering the texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLTextureSampler
```

## Overview

You use texture samplers as material property values with the MDLMaterialProperty class.

## Topics

### Working with Texture Parameters

var texture: MDLTexture?

The texture object that provides image data for sampling.

var hardwareFilter: MDLTextureFilter?

An object that describes filtering modes for sampling from the texture.

var transform: MDLTransform?

The transformation to be applied to texture coordinate data before sampling from the texture.

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

class MDLTextureFilter

A description of filtering modes for a renderer to use when sampling from a texture.

