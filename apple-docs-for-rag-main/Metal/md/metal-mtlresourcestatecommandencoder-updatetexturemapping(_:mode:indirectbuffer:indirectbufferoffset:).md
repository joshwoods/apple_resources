

- Metal
- MTLResourceStateCommandEncoder
-  updateTextureMapping(\_:mode:indirectBuffer:indirectBufferOffset:) 

Instance Method

# updateTextureMapping(\_:mode:indirectBuffer:indirectBufferOffset:)

Encodes a command to update a texture’s memory mappings, specifying the parameters indirectly.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

**Mac Catalyst, macOS**

``` source
optional func updateTextureMapping(
    _ texture: any MTLTexture,
    mode: MTLSparseTextureMappingMode,
    indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int
)
```

**iOS, iPadOS, tvOS, visionOS**

``` source
func updateTextureMapping(
    _ texture: any MTLTexture,
    mode: MTLSparseTextureMappingMode,
    indirectBuffer: any MTLBuffer,
    indirectBufferOffset: Int
)
```

**Required**

## Parameters 

`texture`  

The sparse texture to update.

`mode`  

A mode that indicates whether the method allocates or frees a memory tile in the texture.

`indirectBuffer`  

A buffer that contains an array of mapping arguments that are instances of the MTLMapIndirectArguments structure.

`indirectBufferOffset`  

The offset, in bytes, where the first argument begins in the `indirectBuffer` parameter.

## Discussion

When the GPU executes the command that updates the texture’s memory mapping, the GPU gets details about the region to update from the `indirectBuffer` parameter.

To allocate tiles from the heap, pass MTLSparseTextureMappingMode.map as the `mode` parameter, and to free files back to the heap, pass MTLSparseTextureMappingMode.unmap.

If you encode other commands that use the texture’s contents, such as rendering to the texture or sampling from a texture, synchronize the texture’s mapping updates with those commands to avoid race conditions. See Resource Synchronization.

If you encode commands with multiple resource state passes, synchronize the resources to run the commands in the passes sequentially. See the MTLResourceStateCommandEncoder protocol.

