

- Model I/O
-  MDLMaterialMipMapFilterMode 

Enumeration

# MDLMaterialMipMapFilterMode

Modes for sampling textures at sizes between mipmap levels, used by the mipFilter property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLMaterialMipMapFilterMode
```

## Topics

### Constants

case nearest

Sampling a texture at a size between mipmap levels should return a texel value from the nearest mipmap level.

case linear

Sampling a texture at a size between mipmap levels should linearly interpolate between mipmap levels.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum MDLMaterialTextureWrapMode

Modes for sampling textures at coordinates outside the texture bounds, used by the sWrapMode, tWrapMode, and rWrapMode properties.

enum MDLMaterialTextureFilterMode

Modes for sampling textures at coordinates between texels, used by the minFilter and magFilter properties.

