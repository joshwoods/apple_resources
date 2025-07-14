

- Metal
- MTLBlitCommandEncoder
-  optimizeContentsForCPUAccess(texture:) 

Instance Method

# optimizeContentsForCPUAccess(texture:)

Encodes a command that improves the performance of the CPU’s accesses to a texture.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
func optimizeContentsForCPUAccess(texture: any MTLTexture)
```

**Required**

## Parameters 

`texture`  

A texture the command optimizes.

## Mentioned in 

Optimizing Texture Data

## Discussion

This command can reduce the time it takes the CPU to access a texture. Apps typically run the command for:

- Textures the CPU accesses for an extended period of time

- Textures with a storageMode property that’s MTLStorageMode.shared or MTLStorageMode.managed

When a blit pass runs this command, the GPU only applies lossless changes to the texture’s underlying data.

Note

Optimizing a texture for the CPU may affect the performance of the GPU’s accesses, but the data the GPU retrieves from the texture remains consistent.

## See Also

### Working with Textures on the CPU

func optimizeContentsForCPUAccess(texture: any MTLTexture, slice: Int, level: Int)

Encodes a command that improves the performance of the CPU’s accesses to a specific portion of a texture.

**Required**

