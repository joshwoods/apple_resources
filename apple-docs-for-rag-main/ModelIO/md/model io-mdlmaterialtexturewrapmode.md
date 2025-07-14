

- Model I/O
-  MDLMaterialTextureWrapMode 

Enumeration

# MDLMaterialTextureWrapMode

Modes for sampling textures at coordinates outside the texture bounds, used by the sWrapMode, tWrapMode, and rWrapMode properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLMaterialTextureWrapMode
```

## Topics

### Constants

case clamp

Sampling at any texture coordinate outside the `0.0` to `1.0` range returns the texel color from the nearest edge.

case `repeat`

Sampling at texture coordinates outside the `0.0` to `1.0` range results in a repeated tiling effect.

case mirror

Sampling at texture coordinates outside the `0.0` to `1.0` range results in a mirrored tiling effect.

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

enum MDLMaterialTextureFilterMode

Modes for sampling textures at coordinates between texels, used by the minFilter and magFilter properties.

enum MDLMaterialMipMapFilterMode

Modes for sampling textures at sizes between mipmap levels, used by the mipFilter property.

