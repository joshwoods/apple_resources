

- Metal
- GPU Devices and Work Submission
- MTLCommandBuffer
-  Command Encoder Factory Methods 

API Collection

# Command Encoder Factory Methods

A command encoder defines the actions of a single pass, such as GPU commands that draw, compute, or quickly copy resource data.

## Topics

### Creating Render Encoders

A render encoder creates a render pass that draws graphics with a GPU.

func makeRenderCommandEncoder(descriptor: MTLRenderPassDescriptor) -> (any MTLRenderCommandEncoder)?

Creates a render command encoder from a descriptor.

**Required**

### Creating Parallel Render Encoders

A parallel render encoder creates multiple render encoders that all contribute to a single render pass that draws graphics with a GPU.

func makeParallelRenderCommandEncoder(descriptor: MTLRenderPassDescriptor) -> (any MTLParallelRenderCommandEncoder)?

Creates a parallel render command encoder from a descriptor.

**Required**

### Creating Acceleration Structure Encoders

An acceleration structure encoder creates a pass that builds or refits data for ray tracing with a GPU.

func makeAccelerationStructureCommandEncoder(descriptor: MTLAccelerationStructurePassDescriptor) -> any MTLAccelerationStructureCommandEncoder

Creates a ray-tracing acceleration structure command encoder from a descriptor.

**Required**

func makeAccelerationStructureCommandEncoder() -> (any MTLAccelerationStructureCommandEncoder)?

Creates a ray-tracing acceleration structure command encoder that uses default settings.

**Required**

### Creating Compute Encoders

A compute encoder creates a pass that runs computations in parallel with the GPU.

func makeComputeCommandEncoder(descriptor: MTLComputePassDescriptor) -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder from a descriptor.

**Required**

func makeComputeCommandEncoder() -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder that uses default settings.

**Required**

func makeComputeCommandEncoder(dispatchType: MTLDispatchType) -> (any MTLComputeCommandEncoder)?

Creates a compute command encoder with a dispatch type.

**Required**

enum MTLDispatchType

The type of dispatch method to use when calling encoded functions.

### Creating Blit Encoders

A block information transfer (blit) encoder creates a pass that quickly copies data between GPU resources, including buffers and textures.

func makeBlitCommandEncoder() -> (any MTLBlitCommandEncoder)?

Creates a block information transfer (blit) encoder.

**Required**

func makeBlitCommandEncoder(descriptor: MTLBlitPassDescriptor) -> (any MTLBlitCommandEncoder)?

Creates a block information transfer (blit) encoder from a descriptor.

**Required**

### Creating Resource State Encoders

A resource state encoder creates a pass that manages memory for sparse textures.

func resourceStateCommandEncoder(with: MTLResourceStatePassDescriptor) -> (any MTLResourceStateCommandEncoder)?

Creates a resource state command encoder from a descriptor.

**Required**

func makeResourceStateCommandEncoder() -> (any MTLResourceStateCommandEncoder)?

Creates a resource state command encoder that uses default settings.

**Required**

