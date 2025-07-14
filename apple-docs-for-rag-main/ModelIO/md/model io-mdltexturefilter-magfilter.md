

- Model I/O
- MDLTextureFilter
-  magFilter 

Instance Property

# magFilter

The filter mode for rendering textures at sizes larger than that of the original image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var magFilter: MDLMaterialTextureFilterMode { get set }
```

## Discussion

Texture filtering determines the appearance of a rendered surface when portions of the surface appear larger or smaller than the original texture image. For example, the texture coordinates at a point near the camera may correspond to a small fraction of a texel. A renderer uses the magnification filter to determine the color of the sampled texel at that point.

The default value is MDLMaterialTextureFilterMode.linear, indicating that a renderer should linearly interpolate between texels.

## See Also

### Managing Texture Filter Modes

var minFilter: MDLMaterialTextureFilterMode

The filter mode for rendering textures at sizes smaller than that of the original image.

var mipFilter: MDLMaterialMipMapFilterMode

The filter mode for rendering textures using mipmapping.

