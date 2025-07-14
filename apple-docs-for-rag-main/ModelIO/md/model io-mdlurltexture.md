

- Model I/O
-  MDLURLTexture 

Class

# MDLURLTexture

A lightweight reference to a URL from which to load texture data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLURLTexture
```

## Overview

Unlike the superclass MDLTexture, the MDLURLTexture class loads texel data from the file at that URL only when that data is first referenced, and then caches it for future use.

## Topics

### Creating a URL Texture

init(url: URL, name: String?)

Initializes a texture that loads its texel data from a file at the specified URL.

### Inspecting the Texture URL

var url: URL

The URL from which to load texture data.

## Relationships

### Inherits From

- MDLTexture

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
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

class MDLTextureFilter

A description of filtering modes for a renderer to use when sampling from a texture.

class MDLTextureSampler

An object that pairs a source of texture data with sampling parameters to be used in rendering the texture.

