

- Metal
- MTLRenderCommandEncoder
-  setVertexTextures(\_:range:) 

Instance Method

# setVertexTextures(\_:range:)

Assigns multiple textures to a range of entries in the vertex shader argument table.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func setVertexTextures(
    _ textures: [(any MTLTexture)?],
    range: Range
)
```

## Parameters 

`textures`  

An array of MTLTexture instances the command assigns to entries in the vertex shader argument table for textures.

`range`  

A span of integers that represent the entries in the vertex shader argument table for textures. Each entry stores a record of the corresponding element in `textures`.

## Discussion

By default, the texture at each index is `nil`.

Note

The Objective-C version of this method is setVertexTextures:withRange:.

## See Also

### Assigning Textures

func setVertexTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the vertex shader argument table.

**Required**

