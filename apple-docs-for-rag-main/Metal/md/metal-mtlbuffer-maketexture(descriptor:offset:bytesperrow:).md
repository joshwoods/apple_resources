

- Metal
- MTLBuffer
-  makeTexture(descriptor:offset:bytesPerRow:) 

Instance Method

# makeTexture(descriptor:offset:bytesPerRow:)

Creates a texture that shares its storage with the buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.13+tvOSvisionOS 1.0+

``` source
func makeTexture(
    descriptor: MTLTextureDescriptor,
    offset: Int,
    bytesPerRow: Int
) -> (any MTLTexture)?
```

**Required**

## Parameters 

`descriptor`  

The descriptor that contains the properties of the texture.

`offset`  

The offset, in bytes, from the base address for the first row of texture data.

`bytesPerRow`  

The stride, in bytes, from one row of texture data to the next.

## Return Value

A new texture that shares the buffer’s underlying storage.

## Mentioned in 

Optimizing Texture Data

Developing Metal apps that run in Simulator

## Discussion

This method creates a new MTLTexture instance that uses the same data as the buffer’s. Modifying the buffer also modifies the new texture because they share the same underlying memory.

Note

Metal may not be able to optimize a texture that shares memory with a buffer.

The texture’s resource data is coherent between multiple render passes. However, data accesses within a single render pass may not be coherent due to caching at runtime. For example, a texture from this method may not be able to immediately access new values from a render or kernel function that modifies this buffer.

If this buffer’s storageMode is MTLStorageMode.managed, and a render or kernel function modifies it, the CPU can access the new values through a texture after calling the synchronize(resource:) method. CPU accesses are only coherent between command buffer boundaries. GPU barriers guard a GPU’s accesses to buffers and textures so that each access finishes running before the next one begins.

You can create multiple, nonoverlapping textures that use the same buffer; however, the GPU serializes accesses to those textures.

Tip

You can avoid the GPU’s texture access serialization by creating multiple buffers and then creating a texture from each buffer with this method.

To create a linear texture, you need to:

- Align the `offset` and `bytesPerRow` parameters to the value that the minimumLinearTextureAlignment(for:) method returns.

- Set the `bytesPerRow` parameter to a value greater than or equal to the number of bytes in one row of pixels — the product of the row’s width, in pixels, and the size of one pixel, in bytes.

Additionally, creating a linear texture from this method adds the following restrictions for the `descriptor` parameter’s properties:

| Property | Acceptable values for a linear texture |
|----|----|
| textureType | MTLTextureType.type2D or MTLTextureType.typeTextureBuffer |
| depth | `1` |
| arrayLength | `1` |
| mipmapLevelCount | `1` |
| sampleCount | `1` |
| usage | The renderTarget value if the MTLDevice instance supports MTLGPUFamily.apple1 (see supportsFamily(_:)), or any other MTLTextureUsage value |
| storageMode | The same value as this buffer’s storageMode property (see Resource Fundamentals) |
| pixelFormat | Any ordinary or packed color MTLPixelFormat, except MTLPixelFormat.gbgr422 and MTLPixelFormat.bgrg422 |

Samplers can use any MTLSamplerAddressMode to sample linear textures from this method on any device that supports the MTLGPUFamily.apple2 feature family or later.

Note

For devices that support only the MTLGPUFamily.apple1 feature family, samplers can only use MTLSamplerAddressMode.clampToEdge to sample a linear texture.

