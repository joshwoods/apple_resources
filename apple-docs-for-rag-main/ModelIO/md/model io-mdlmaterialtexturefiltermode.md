

- Model I/O
-  MDLMaterialTextureFilterMode 

Enumeration

# MDLMaterialTextureFilterMode

Modes for sampling textures at coordinates between texels, used by the minFilter and magFilter properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLMaterialTextureFilterMode
```

## Topics

### Constants

case nearest

Sampling at texture coordinates between texels should return the value of the nearest texel.

case linear

Sampling at texture coordinates between texels should linearly interpolate between texel values.

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

enum MDLMaterialMipMapFilterMode

Modes for sampling textures at sizes between mipmap levels, used by the mipFilter property.

