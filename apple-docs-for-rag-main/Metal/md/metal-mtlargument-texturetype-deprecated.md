

- Metal
- MTLArgument
-  textureType Deprecated

Instance Property

# textureType

The texture type of a texture argument.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var textureType: MTLTextureType { get }
```

## Discussion

For information on possible values, see MTLTextureType. If the argument is not a texture, querying this property is a fatal error.

## See Also

### Describing a Texture Argument

var textureDataType: MTLDataType

The data type of a texture argument.

Deprecated

var isDepthTexture: Bool

A Boolean value that indicates whether the texture is a depth texture.

Deprecated

