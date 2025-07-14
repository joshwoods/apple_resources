

- Model I/O
- MDLTextureFilter
-  sWrapMode 

Instance Property

# sWrapMode

The coordinate wrapping mode for texture t-coordinates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var sWrapMode: MDLMaterialTextureWrapMode { get set }
```

## Discussion

Texture coordinates canonically range from `0.0` to `1.0`; wrap mode determines the behavior for samples from outside that range. For details, see MDLMaterialTextureWrapMode.

The s-coordinate is the first (or only) value in a set of texture coordinates, used with one-, two-, and three-dimensional textures.

## See Also

### Managing Texture Coordinate Wrap Modes

var tWrapMode: MDLMaterialTextureWrapMode

The coordinate wrapping mode for texture t-coordinates.

var rWrapMode: MDLMaterialTextureWrapMode

The coordinate wrapping mode for texture r-coordinates.

