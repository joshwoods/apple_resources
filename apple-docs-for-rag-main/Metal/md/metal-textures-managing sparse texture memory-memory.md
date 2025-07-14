

- Metal
- Textures
-  Managing Sparse Texture Memory 

Article

# Managing Sparse Texture Memory

Take direct control of memory allocation for texture data by using sparse textures.

## Overview

When you create a texture, by default, Metal allocates memory to hold the texture’s pixel data. In some cases, such as when you’re implementing texture streaming, you generally use only a fraction of this memory. When you use sparse textures, you take ownership of memory management for texture data and decide when to allocate and deallocate memory for a texture. In this way, sparse textures help you to use memory more efficiently.

To use sparse textures, allocate a sparse heap from which to allocate memory, and then create sparse textures from this heap. Initially, a texture has no storage. To add storage to a region inside the texture, ask the GPU to map memory from the heap for that region. A *sparse tile* is a memory allocation (as opposed to memory tiles a GPU uses for tile-based rendering). Sparse tiles are conceptually similar to virtual memory pages. When you don’t need a region to have storage, you can unmap its sparse tile and recover that memory.

Because sparse textures work closely with texture mipmaps, you should be familiar with mipmaps before using sparse textures. For more information, see Improving Texture Sampling Quality and Performance with Mipmaps.

### Check for Sparse Texture Support

Not all GPUs support sparse textures. Check for support on the device object before attempting to use sparse textures:

```
- (Boolean) supportsSparseTextures
{
    return [_device supportsFamily: MTLGPUFamilyApple6 ];
}
```

## See Also

### Sparse Textures

Creating Sparse Heaps and Sparse Textures

Allocate memory for sparse textures by creating a sparse heap.

Converting Between Pixel Regions and Sparse Tile Regions

Learn how a sparse texture’s contents are organized in memory.

Assigning Memory to Sparse Textures

Use a resource state encoder to allocate and deallocate sparse tiles for a sparse texture.

Reading and Writing to Sparse Textures

Decide how to handle access to unmapped texture regions.

Estimating How Often a Texture Region Is Accessed

Use texture access patterns to determine when you need to map a texture region.

class MTLResourceStatePassDescriptor

A configuration for a resource state pass, used to create a resource state command encoder.

class MTLResourceStatePassSampleBufferAttachmentDescriptor

A description of where to store GPU counter information at the start and end of a resource state pass.

class MTLResourceStatePassSampleBufferAttachmentDescriptorArray

An array of sample buffer attachments for a resource state pass.

protocol MTLResourceStateCommandEncoder

An encoder that encodes commands that modify resource configurations.

struct MTLMapIndirectArguments

The data layout for mapping sparse texture regions when using indirect commands.

