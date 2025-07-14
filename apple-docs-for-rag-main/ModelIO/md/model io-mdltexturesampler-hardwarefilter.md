

- Model I/O
- MDLTextureSampler
-  hardwareFilter 

Instance Property

# hardwareFilter

An object that describes filtering modes for sampling from the texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var hardwareFilter: MDLTextureFilter? { get set }
```

## Discussion

Filtering modes specify the behavior of texture sampling at different sizes and texture coordinates.

## See Also

### Working with Texture Parameters

var texture: MDLTexture?

The texture object that provides image data for sampling.

var transform: MDLTransform?

The transformation to be applied to texture coordinate data before sampling from the texture.

