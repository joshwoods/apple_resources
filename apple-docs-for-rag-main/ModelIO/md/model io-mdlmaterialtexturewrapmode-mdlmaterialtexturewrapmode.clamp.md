

- Model I/O
- MDLMaterialTextureWrapMode
-  MDLMaterialTextureWrapMode.clamp 

Case

# MDLMaterialTextureWrapMode.clamp

Sampling at any texture coordinate outside the `0.0` to `1.0` range returns the texel color from the nearest edge.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case clamp
```

## See Also

### Constants

case `repeat`

Sampling at texture coordinates outside the `0.0` to `1.0` range results in a repeated tiling effect.

case mirror

Sampling at texture coordinates outside the `0.0` to `1.0` range results in a mirrored tiling effect.

