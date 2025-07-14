

- Model I/O
-  MDLNoiseTexture 

Class

# MDLNoiseTexture

A generator of texel data that creates a field of random noise.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLNoiseTexture
```

## Overview

Like other procedural MDLTexture subclasses, the MDLNoiseTexture class generates texel data only when that data is first referenced, and then caches it for future use.

## Topics

### Creating a Noise Texture

init(scalarNoiseWithSmoothness: Float, name: String?, textureDimensions: vector_int2, channelCount: Int32, channelEncoding: MDLTextureChannelEncoding, grayscale: Bool)

Initializes a noise texture that creates random color noise.

init(vectorNoiseWithSmoothness: Float, name: String?, textureDimensions: vector_int2, channelEncoding: MDLTextureChannelEncoding)

Initializes a noise texture that creates random directional noise.

### Initializers

init(cellularNoiseWithFrequency: Float, name: String?, textureDimensions: vector_int2, channelEncoding: MDLTextureChannelEncoding)

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

