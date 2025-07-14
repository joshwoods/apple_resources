

- Metal
- GPU Devices and Work Submission
- MTLDevice
-  Resource Creation 

API Collection

# Resource Creation

Load assets with input/output queues and make various resource instances, such as buffers, textures, acceleration structures, and memory heaps.

## Topics

### Working with Resource Heaps

func makeHeap(descriptor: MTLHeapDescriptor) -> (any MTLHeap)?

Creates a new GPU heap instance.

**Required**

func heapBufferSizeAndAlign(length: Int, options: MTLResourceOptions) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of a buffer if you create it from a heap.

**Required**

func heapTextureSizeAndAlign(descriptor: MTLTextureDescriptor) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of a texture if you create it from a heap.

**Required**

func heapAccelerationStructureSizeAndAlign(size: Int) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap.

**Required**

func heapAccelerationStructureSizeAndAlign(descriptor: MTLAccelerationStructureDescriptor) -> MTLSizeAndAlign

Returns the size and alignment, in bytes, of an acceleration structure if you create it from a heap with a descriptor.

**Required**

struct MTLSizeAndAlign

The size and alignment of a resource, in bytes.

### Creating Buffers

var maxBufferLength: Int

The largest amount of memory, in bytes, that a GPU device can allocate to a buffer instance.

**Required**

func makeBuffer(length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Creates a buffer the method clears with zero values.

**Required**

func makeBuffer(bytes: UnsafeRawPointer, length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Allocates a new buffer of a given length and initializes its contents by copying existing data into it.

**Required**

func makeBuffer(bytesNoCopy: UnsafeMutableRawPointer, length: Int, options: MTLResourceOptions, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?) -> (any MTLBuffer)?

Creates a buffer that wraps an existing contiguous memory allocation.

**Required**

### Creating Textures

func makeTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a new texture instance.

**Required**

func makeTexture(descriptor: MTLTextureDescriptor, iosurface: IOSurfaceRef, plane: Int) -> (any MTLTexture)?

Creates a texture instance that uses I/O surface to store its underlying data.

**Required**

func makeSharedTexture(descriptor: MTLTextureDescriptor) -> (any MTLTexture)?

Creates a texture that you can share across process boundaries.

**Required**

func makeSharedTexture(handle: MTLSharedTextureHandle) -> (any MTLTexture)?

Creates a texture that references a shared texture.

**Required**

func minimumLinearTextureAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a linear texture from a buffer.

**Required**

func minimumTextureBufferAlignment(for: MTLPixelFormat) -> Int

Returns the minimum alignment the GPU device requires to create a texture buffer from a buffer.

**Required**

### Creating Samplers

func supportsTextureSampleCount(Int) -> Bool

Returns a Boolean value that indicates whether the GPU can sample a texture with a specific number of sample points.

**Required**

func makeSamplerState(descriptor: MTLSamplerDescriptor) -> (any MTLSamplerState)?

Creates a sampler state instance.

**Required**

func getDefaultSamplePositions(sampleCount: Int) -> [MTLSamplePosition]

Returns the default sample locations based on the number of samples.

### Working with Sparse Textures

func sparseTileSize(textureType: MTLTextureType, pixelFormat: MTLPixelFormat, sampleCount: Int, sparsePageSize: MTLSparsePageSize) -> MTLSize

Returns the dimensions of a sparse tile for a texture that has a specific sparse page size.

**Required**

func sparseTileSize(with: MTLTextureType, pixelFormat: MTLPixelFormat, sampleCount: Int) -> MTLSize

Returns the dimensions of a sparse tile for a texture.

**Required**

func sparseTileSizeInBytes(sparsePageSize: MTLSparsePageSize) -> Int

Returns the size, in bytes, of a sparse tile the GPU device creates with a specific page size.

**Required**

var sparseTileSizeInBytes: Int

Returns the size, in bytes, of a sparse tile the GPU device creates using a default page size.

**Required**

func convertSparsePixelRegions(UnsafePointer&lt;MTLRegion>, toTileRegions: UnsafeMutablePointer&lt;MTLRegion>, withTileSize: MTLSize, alignmentMode: MTLSparseTextureRegionAlignmentMode, numRegions: Int)

Converts a list of sparse pixel regions to tile regions.

func convertSparseTileRegions(UnsafePointer&lt;MTLRegion>, toPixelRegions: UnsafeMutablePointer&lt;MTLRegion>, withTileSize: MTLSize, numRegions: Int)

Converts a list of sparse tile regions to pixel regions.

enum MTLSparsePageSize

The page size options, in kilobytes, for sparse textures.

enum MTLSparseTextureRegionAlignmentMode

Options used when converting between a pixel-based region within a texture to a tile-based region.

### Creating Acceleration Structures for Ray Tracing

func makeAccelerationStructure(descriptor: MTLAccelerationStructureDescriptor) -> (any MTLAccelerationStructure)?

Creates a new ray-tracing acceleration structure from a descriptor.

**Required**

func makeAccelerationStructure(size: Int) -> (any MTLAccelerationStructure)?

Creates a new acceleration structure with a specific size.

**Required**

func accelerationStructureSizes(descriptor: MTLAccelerationStructureDescriptor) -> MTLAccelerationStructureSizes

Returns the buffer sizes the GPU device needs to build, refit, and store an acceleration structure.

**Required**

struct MTLAccelerationStructureSizes

The expected sizes for a ray-tracing acceleration structure.

### Creating Argument Buffer Encoders

var argumentBuffersSupport: MTLArgumentBuffersTier

Returns the GPU device’s support tier for argument buffers.

**Required**

var maxArgumentBufferSamplerCount: Int

The maximum number of unique argument buffer samplers per app.

**Required**

func makeArgumentEncoder(arguments: [MTLArgumentDescriptor]) -> (any MTLArgumentEncoder)?

Creates a new argument encoder for an array of arguments.

**Required**

func makeArgumentEncoder(bufferBinding: any MTLBufferBinding) -> any MTLArgumentEncoder

Creates a new argument encoder for a buffer binding.

**Required**

### Creating Fences and Events

func makeFence() -> (any MTLFence)?

Creates a new memory fence instance.

**Required**

func makeEvent() -> (any MTLEvent)?

Creates a new event instance that you can use to synchronize commands and resources within the same GPU device.

**Required**

func makeSharedEvent() -> (any MTLSharedEvent)?

Creates a new shared event instance that you can use to synchronize commands and resources across different GPU devices.

**Required**

func makeSharedEvent(handle: MTLSharedEventHandle) -> (any MTLSharedEvent)?

Recreates a shared event from a handle.

**Required**

### Creating Rasterization Rate Maps

func supportsRasterizationRateMap(layerCount: Int) -> Bool

Returns a Boolean value that indicates whether the GPU can create a rasterization rate map with a specific number of layers.

**Required**

func makeRasterizationRateMap(descriptor: MTLRasterizationRateMapDescriptor) -> (any MTLRasterizationRateMap)?

Creates a rasterization rate map instance.

**Required**

## See Also

### Working with GPU Devices

Device Inspection

Locate and identify a GPU and the features it supports, and sample its counters.

Work Submission

Create queues that submit work to the GPU or load assets into GPU resources, and indirect command buffers that group your frequent commands together.

Pipeline State Creation

Create pipeline states for render and compute passes, samplers, depth and stencil states, and indirect command buffers.

Shader Library and Archive Creation

Create static and dynamic shader libraries, and binary shader archives.

