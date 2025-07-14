

- Metal
- MTLRenderCommandEncoder
-  setObjectTextures(\_:range:) 

Instance Method

# setObjectTextures(\_:range:)

Assigns multiple textures to a range of entries in the object shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS

``` source
func setObjectTextures(
    _ textures: [(any MTLTexture)?],
    range: Range
)
```

## Parameters 

`textures`  

An array of MTLTexture instances the command assigns to entries in the object shader argument table for textures.

`range`  

A span of integers that represent the entries in the object shader argument table for textures. Each entry stores a record of the corresponding element in `textures`.

## Discussion

By default, the texture at each index is `nil`.

Note

The Objective-C version of this method is setObjectTextures:withRange:.

## See Also

### Assigning Textures for Object Shaders

func setObjectTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the object shader argument table.

**Required**

