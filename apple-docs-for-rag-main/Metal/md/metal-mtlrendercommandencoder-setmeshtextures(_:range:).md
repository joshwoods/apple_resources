

- Metal
- MTLRenderCommandEncoder
-  setMeshTextures(\_:range:) 

Instance Method

# setMeshTextures(\_:range:)

Assigns multiple textures to a range of entries in the mesh shader argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS

``` source
func setMeshTextures(
    _ textures: [(any MTLTexture)?],
    range: Range
)
```

## Parameters 

`textures`  

An array of MTLTexture instances the command assigns to entries in the mesh shader argument table for textures.

`range`  

A span of integers that represent the entries in the mesh shader argument table for textures. Each entry stores a record of the corresponding element in `textures`.

## Discussion

By default, the texture at each index is `nil`.

Note

The Objective-C version of this method is setMeshTextures:withRange:.

## See Also

### Assigning Textures for Mesh Shaders

func setMeshTexture((any MTLTexture)?, index: Int)

Assigns a texture to an entry in the mesh shader argument table.

**Required**

