

- Metal
- MTLArgumentEncoder
-  setTextures(\_:range:) 

Instance Method

# setTextures(\_:range:)

Encodes references to an array of textures into the argument buffer.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+tvOS 11.0+visionOS

``` source
func setTextures(
    _ textures: [(any MTLTexture)?],
    range: Range
)
```

## Parameters 

`textures`  

An array of textures the method encodes.

`range`  

A range of indices within the argument buffer for each element in `textures`. The values correspond to either the index IDs of declarations in Metal Shading Language (MSL) or the index property of MTLArgumentDescriptor instances.

## See Also

### Encoding Textures

func setTexture((any MTLTexture)?, index: Int)

Encodes a reference to a texture into the argument buffer.

**Required**

