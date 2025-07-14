

- Metal
- Textures
-  Creating Sparse Heaps and Sparse Textures 

Article

# Creating Sparse Heaps and Sparse Textures

Allocate memory for sparse textures by creating a sparse heap.

## Overview

*Sparse heaps* are MTLHeap objects that create sparse textures and provide memory for them. Unlike with a standard heap, you use a sparse heap only to create sparse textures and allocate storage for texture data. You allocate memory when you create the heap, and later, as needed, map or unmap portions of the heap’s memory to textures. Memory is mapped in larger chunks called *sparse tiles*. The size of sparse tiles (in bytes) is determined by the device object.

### Create a Sparse Heap

Create a MTLHeapDescriptor object and set its type to MTLHeapType.sparse. You must allocate sparse heaps with the MTLStorageMode.private storage mode. Specify the heap’s size as a multiple of the sparse tile size. To get the tile size, read the sparseTileSizeInBytes property on the MTLDevice object that you’re using to create the heap.

The code below creates a new sparse heap, rounding the heap size up to the tile size.

- Swift
- Objective-C

```
let sparseHeapSizeInBytes = 256 * 1024 * 1024
let sparseTileSize = device.sparseTileSizeInBytes
let alignedHeapSize = ((sparseHeapSizeInBytes + sparseTileSize - 1) / sparseTileSize) * sparseTileSize

let descriptor = MTLHeapDescriptor()
descriptor.type = .sparse
descriptor.storageMode = .private
descriptor.size = alignedHeapSize

let sparseHeap = device.makeHeap(descriptor: descriptor)
```

```
const int sparseHeapSizeInBytes = 256 * 1024 * 1024;
int sparseTileSize = _device.sparseTileSizeInBytes;
int alignedHeapSize = ((sparseHeapSizeInBytes + sparseTileSize-1) / sparseTileSize) * sparseTileSize;

MTLHeapDescriptor* descriptor = [MTLHeapDescriptor new];
descriptor.type = MTLHeapTypeSparse;
descriptor.storageMode = MTLStorageModePrivate;
descriptor.size = alignedHeapSize;

id sparseHeap = [_device newHeapWithDescriptor: descriptor];
```

Specify a heap size that’s appropriate for your app, based on how many textures you’ve, how large those textures are, and your image-quality goals. You may need to experiment to determine the best size. The heap should be large enough that your app doesn’t need to unmap sparse tiles frequently and doesn’t suffer from image-quality problems. Unless you need finer-grained control of how different collections of textures are allocated in memory, allocate a single sparse heap and use it to manage all of your app’s texture memory.

### Create a Sparse Texture

All textures that you create on a sparse heap are sparse textures. When you create textures on heaps, you must use the same storage mode as you used to create the sparse heap, as shown in the code below:

- Swift
- Objective-C

```
let textureDescriptor = MTLTextureDescriptor.texture2DDescriptor(pixelFormat: .bgra8Unorm_srgb,
                                                                 width: 1024, height: 1024, mipmapped: true)
textureDescriptor.storageMode = sparseHeap.storageMode
let sparseTexture = sparseHeap.makeTexture(descriptor: textureDescriptor)
```

```
MTLTextureDescriptor *textureDescriptor =
    [MTLTextureDescriptor texture2DDescriptorWithPixelFormat:(MTLPixelFormatBGRA8Unorm_sRGB)
         width:1024
        height:1024
     mipmapped:YES];
textureDescriptor.storageMode = _sparseHeap.storageMode;
id sparseTexture =  [_sparseHeap newTextureWithDescriptor:textureDescriptor];
```

When you create a sparse texture, no memory is allocated for it. It can’t store any pixel data until you map sparse tiles on the heap to regions inside the texture. For more information about mapping and unmapping sparse tiles, see Assigning Memory to Sparse Textures. For more information about how sparse textures behave when you access them, see Reading and Writing to Sparse Textures.

## See Also

### Sparse Textures

Managing Sparse Texture Memory

Take direct control of memory allocation for texture data by using sparse textures.

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

