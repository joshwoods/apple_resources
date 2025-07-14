

- Metal
- MTLArgumentEncoder
-  setTexture(\_:index:) 

Instance Method

# setTexture(\_:index:)

Encodes a reference to a texture into the argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func setTexture(
    _ texture: (any MTLTexture)?,
    index: Int
)
```

**Required**

## Parameters 

`texture`  

A texture the method encodes.

`index`  

The index of a texture within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## See Also

### Encoding Textures

func setTextures([(any MTLTexture)?], range: Range&lt;Int>)

Encodes references to an array of textures into the argument buffer.

