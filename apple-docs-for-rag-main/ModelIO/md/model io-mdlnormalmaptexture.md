

- Model I/O
-  MDLNormalMapTexture 

Class

# MDLNormalMapTexture

A generator of texel data that computes a normal map from a supplied texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLNormalMapTexture
```

## Overview

This class examines the shapes of contrasting areas in an input texture to generate a normal map that produces an embossed appearance when rendered with lighting. The figure below shows the normal map generated from an example texture and the effect of using this normal map with lighting in a typical renderer.

Like other procedural MDLTexture subclasses, the MDLNormalMapTexture class generates texel data only when that data is first referenced, and caches it for future use.

## Topics

### Creating a Normal Map Texture

init(byGeneratingNormalMapWith: MDLTexture, name: String?, smoothness: Float, contrast: Float)

Initializes a normal map to be generated from the specified texture.

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

class MDLSkyCubeTexture

A generator of texel data that creates cube textures using a physically realistic simulation of the sunlit sky.

class MDLURLTexture

A lightweight reference to a URL from which to load texture data.

class MDLTextureFilter

A description of filtering modes for a renderer to use when sampling from a texture.

class MDLTextureSampler

An object that pairs a source of texture data with sampling parameters to be used in rendering the texture.

