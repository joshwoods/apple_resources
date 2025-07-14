

- Model I/O
-  MDLColorSwatchTexture 

Class

# MDLColorSwatchTexture

A generator of texel data that creates a gradient between two specified colors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLColorSwatchTexture
```

## Overview

A MDLColorSwatchTexture object procedurally generates texel data by creating a gradient between two colors. Like other procedural MDLTexture subclasses, the MDLColorSwatchTexture class generates texel data only when that data is first referenced, and caches it for future use.

## Topics

### Creating a Color Swatch Texture

init(colorGradientFrom: CGColor, to: CGColor, name: String?, textureDimensions: vector_int2)

Initializes a texture that creates a vertical gradient between two colors.

init(colorTemperatureGradientFrom: Float, toColorTemperature: Float, name: String?, textureDimensions: vector_int2)

Initializes a texture that creates a vertical gradient between two color temperatures.

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

