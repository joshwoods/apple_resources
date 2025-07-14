

- Model I/O
- MDLTextureSampler
-  transform 

Instance Property

# transform

The transformation to be applied to texture coordinate data before sampling from the texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var transform: MDLTransform? { get set }
```

## Discussion

Use this property to translate, scale, or rotate a texture relative to the surfaces it’s rendered on.

## See Also

### Working with Texture Parameters

var texture: MDLTexture?

The texture object that provides image data for sampling.

var hardwareFilter: MDLTextureFilter?

An object that describes filtering modes for sampling from the texture.

