

- Metal
- MTLTextureReferenceType
-  access 

Instance Property

# access

The texture’s read/write access to the argument.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var access: MTLBindingAccess { get }
```

## Discussion

This property indicates the type of access qualifiers (read-only, write-only, or read-write) used in the Metal shading language code. For information on possible values, see MTLArgumentAccess.

## See Also

### Describing the Texture

var textureType: MTLTextureType

The texture type of the texture.

var textureDataType: MTLDataType

The data type of the texture.

var isDepthTexture: Bool

A Boolean value that indicates whether the texture is a depth texture.

