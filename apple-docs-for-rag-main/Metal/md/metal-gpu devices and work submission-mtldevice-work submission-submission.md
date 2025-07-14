

- Metal
- GPU Devices and Work Submission
- MTLDevice
-  Work Submission 

API Collection

# Work Submission

Create queues that submit work to the GPU or load assets into GPU resources, and indirect command buffers that group your frequent commands together.

## Topics

### Creating Command Queues

Command queues encode and submit work to the GPU, which include render, compute, and blit passes.

func makeCommandQueue() -> (any MTLCommandQueue)?

Creates a queue you use to submit rendering and computation commands to a GPU.

**Required**

func makeCommandQueue(maxCommandBufferCount: Int) -> (any MTLCommandQueue)?

Creates a queue you use to submit rendering and computation commands to a GPU that has a fixed number of uncompleted command buffers.

**Required**

### Creating Residency Sets

A residency set makes a group of resources, such as buffers, textures, and heaps, accessible to a GPU for your command buffers and their shaders.

func makeResidencySet(descriptor: MTLResidencySetDescriptor) throws -> any MTLResidencySet

Creates a residency set, which can move resources in and out of memory residency.

**Required**

### Creating I/O Command Queues

Input/Output command queues load assets from the file system into textures, GPU buffers, and traditional CPU buffers.

func makeIOCommandQueue(descriptor: MTLIOCommandQueueDescriptor) throws -> any MTLIOCommandQueue

Creates an input/output command queue you use to submit commands that load assets from the file system into GPU resources or system memory.

**Required**

### Creating I/O File Handles

Input/Output file handles each represent an asset in the file system that an I/O command queue loads into a resource for your app.

func makeIOFileHandle(url: URL) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a file at a URL.

**Required**

func makeIOFileHandle(url: URL, compressionMethod: MTLIOCompressionMethod) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a compressed file at a URL.

**Required**

func makeIOHandle(url: URL) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a file at a URL.

**Required**

Deprecated

func makeIOHandle(url: URL, compressionMethod: MTLIOCompressionMethod) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a compressed file at a URL.

**Required**

Deprecated

### Creating Indirect Command Buffers

Indirect command buffers (ICBs) store commands that you can reuse throughout your app’s lifetime, instead of encoding the same commands repeatedly.

func makeIndirectCommandBuffer(descriptor: MTLIndirectCommandBufferDescriptor, maxCommandCount: Int, options: MTLResourceOptions) -> (any MTLIndirectCommandBuffer)?

Creates an indirect command buffer instance.

**Required**

## See Also

### Working with GPU Devices

Device Inspection

Locate and identify a GPU and the features it supports, and sample its counters.

Pipeline State Creation

Create pipeline states for render and compute passes, samplers, depth and stencil states, and indirect command buffers.

Resource Creation

Load assets with input/output queues and make various resource instances, such as buffers, textures, acceleration structures, and memory heaps.

Shader Library and Archive Creation

Create static and dynamic shader libraries, and binary shader archives.

