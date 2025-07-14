

- Model I/O
- MDLMaterialTextureWrapMode
-  MDLMaterialTextureWrapMode.repeat 

Case

# MDLMaterialTextureWrapMode.repeat

Sampling at texture coordinates outside the `0.0` to `1.0` range results in a repeated tiling effect.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case `repeat`
```

## Discussion

This effect disregards the whole part of a texture coordinate. For example, sampling at a coordinate value of `2.7` or `5.7` returns the texel color for the coordinate value of `0.7`. The visual effect of this mode is to repeat the texture image endlessly across a surface rendered with the texture.

## See Also

### Constants

case clamp

Sampling at any texture coordinate outside the `0.0` to `1.0` range returns the texel color from the nearest edge.

case mirror

Sampling at texture coordinates outside the `0.0` to `1.0` range results in a mirrored tiling effect.

