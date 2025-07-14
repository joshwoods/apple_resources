

- Metal
- MTLRenderCommandEncoder
-  setFragmentTexture(\_:index:) 

Instance Method

# setFragmentTexture(\_:index:)

Assigns a texture to an entry in the fragment shader argument table.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setFragmentTexture(
    _ texture: (any MTLTexture)?,
    index: Int
)
```

**Required**

## Parameters 

`texture`  

An MTLTexture instance the command assigns to an entry in the fragment shader argument table for textures.

`index`  

An integer that represents the entry in the fragment shader argument table for textures that stores a record of `texture`.

## Discussion

By default, the texture at each index is `nil`.

## See Also

### Assigning Textures

func setFragmentTextures([(any MTLTexture)?], range: Range&lt;Int>)

Assigns multiple textures to a range of entries in the fragment shader argument table.

