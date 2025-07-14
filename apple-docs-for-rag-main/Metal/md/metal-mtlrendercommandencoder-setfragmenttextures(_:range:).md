

- Metal
- MTLRenderCommandEncoder
-  setFragmentTextures(\_:range:) 

Instance Method

# setFragmentTextures(\_:range:)

Assigns multiple textures to a range of entries in the fragment shader argument table.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func setFragmentTextures(
    _ textures: [(any MTLTexture)?],
    range: Range
)
```

## Parameters 

`textures`  

An array of MTLTexture instances the command assigns to entries in the fragment shader argument table for textures.

`range`  

A span of integers that represent the entries in the fragment shader argument table for textures. Each entry stores a record of the corresponding element in `textures`.

## Discussion

By default, the texture at each index is `nil`.

Note

The Objective-C version of this method is setFragmentTextures:withRange:.

## See Also

### Assigning Textures

func setFragmentTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the fragment shader argument table.

**Required**

