

- Metal
- MTLBlitCommandEncoder
-  optimizeContentsForGPUAccess(texture:slice:level:) 

Instance Method

# optimizeContentsForGPUAccess(texture:slice:level:)

Encodes a command that improves the performance of the GPU’s accesses to a specific portion of a texture.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func optimizeContentsForGPUAccess(
    texture: any MTLTexture,
    slice: Int,
    level: Int
)
```

**Required**

## Parameters 

`texture`  

A texture the command optimizes.

`slice`  

A slice within `texture`.

`level`  

A mipmap level within `texture`.

## Mentioned in 

Optimizing Texture Data

## Discussion

This command can reduce the time it takes the GPU to access a texture. Apps typically run the command for:

- Textures the GPU accesses for an extended period of time

- Textures with a storageMode property that’s MTLStorageMode.shared or MTLStorageMode.managed

When a blit pass runs this command, the GPU only applies lossless changes to the texture’s underlying data.

Note

Optimizing a texture for the GPU may affect the performance of the CPU’s accesses, but the data the CPU retrieves from the texture remains consistent.

## See Also

### Working with Textures on the GPU

func optimizeContentsForGPUAccess(texture: any MTLTexture)

Encodes a command that improves the performance of the GPU’s accesses to a texture.

**Required**

