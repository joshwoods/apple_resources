

- Metal
- MTLRenderCommandEncoder
-  setTileTexture(\_:index:) 

Instance Method

# setTileTexture(\_:index:)

Assigns a texture to an entry in the tile shader argument table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func setTileTexture(
    _ texture: (any MTLTexture)?,
    index: Int
)
```

**Required**

## Parameters 

`texture`  

An MTLTexture instance the command assigns to an entry in the tile shader argument table for textures.

`index`  

An integer that represents the entry in the tile shader argument table for textures that stores a record of `texture`.

## Discussion

By default, the texture at each index is `nil`.

## See Also

### Assigning Textures

func setTileTextures([(any MTLTexture)?], range: Range&lt;Int>)

Assigns multiple textures to a range of entries in the tile shader argument table.

