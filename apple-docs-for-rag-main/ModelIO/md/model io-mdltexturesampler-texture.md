

- Model I/O
- MDLTextureSampler
-  texture 

Instance Property

# texture

The texture object that provides image data for sampling.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var texture: MDLTexture? { get set }
```

## Discussion

A MDLTexture object describes texture image data.

## See Also

### Working with Texture Parameters

var hardwareFilter: MDLTextureFilter?

An object that describes filtering modes for sampling from the texture.

var transform: MDLTransform?

The transformation to be applied to texture coordinate data before sampling from the texture.

