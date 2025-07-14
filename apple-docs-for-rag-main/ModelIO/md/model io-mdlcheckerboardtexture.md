

- Model I/O
-  MDLCheckerboardTexture 

Class

# MDLCheckerboardTexture

A generator of texel data that creates a checkerboard pattern with two specified colors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLCheckerboardTexture
```

## Overview

Like other procedural MDLTexture subclasses, the MDLCheckerboardTexture class generates texel data only when that data is first referenced, and then caches it for future use.

## Topics

### Creating a Checkerboard Texture

init(divisions: Float, name: String?, dimensions: vector_int2, channelCount: Int32, channelEncoding: MDLTextureChannelEncoding, color1: CGColor, color2: CGColor)

Initializes a checkerboard texture with the specified colors and other properties.

### Configuring the Checkerboard Pattern

var color1: CGColor?

The color for half of the squares in the checkerboard pattern.

var color2: CGColor?

The color for the other half of the squares in the checkerboard pattern.

var divisions: Float

The number of squares along each dimension in the checkerboard pattern.

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

class MDLTextureSampler

An object that pairs a source of texture data with sampling parameters to be used in rendering the texture.

