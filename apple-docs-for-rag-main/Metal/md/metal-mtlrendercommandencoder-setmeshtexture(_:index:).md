

- Metal
- MTLRenderCommandEncoder
-  setMeshTexture(\_:index:) 

Instance Method

# setMeshTexture(\_:index:)

Assigns a texture to an entry in the mesh shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func setMeshTexture(
    _ texture: (any MTLTexture)?,
    index: Int
)
```

**Required**

## Parameters 

`texture`  

An MTLTexture instance the command assigns to an entry in the mesh shader argument table for textures.

`index`  

An integer that represents the entry in the mesh shader argument table for textures that stores a record of `texture`.

## Discussion

By default, the texture at each index is `nil`.

## See Also

### Assigning Textures for Mesh Shaders

func setMeshTextures([(any MTLTexture)?], range: Range&lt;Int>)

Assigns multiple textures to a range of entries in the mesh shader argument table.

