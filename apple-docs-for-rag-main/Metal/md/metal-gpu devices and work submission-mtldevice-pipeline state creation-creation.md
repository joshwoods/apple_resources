

- Metal
- GPU Devices and Work Submission
- MTLDevice
-  Pipeline State Creation 

API Collection

# Pipeline State Creation

Create pipeline states for render and compute passes, samplers, depth and stencil states, and indirect command buffers.

## Overview

Use these methods to create instances of various state types for a render or compute pass (see Render Passes and Compute Passes, respectively).

You can create multiple MTLRenderPipelineState instances for a single render pass encoder (MTLRenderCommandEncoder) that each apply to different types of render commands. For example, a single render pass can render primitives with vertices, then meshes, and finish with a tile shader command, each with a different pipeline. To create these pipelines, configure instances of MTLRenderPipelineDescriptor, MTLMeshRenderPipelineDescriptor, and MTLTileRenderPipelineDescriptor. Then pass those descriptors to the makeRenderPipelineState(descriptor:completionHandler:), makeRenderPipelineState(descriptor:options:completionHandler:) and makeRenderPipelineState(tileDescriptor:options:completionHandler:) methods (or a counterpart method), respectively.

Important

Only create reflection (see MTLRenderPipelineReflection) instances if you need them, because each one can require a significant amount of memory.

## Topics

### Creating Render Pipeline States with Vertex Shaders

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, completionHandler: MTLNewRenderPipelineStateCompletionHandler)

Asynchronously creates a render pipeline state.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedRenderPipelineReflection?>?) throws -> any MTLRenderPipelineState

Synchronously creates a render pipeline state and reflection information.

**Required**

func makeRenderPipelineState(descriptor: MTLRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a render pipeline state and reflection information.

**Required** Default implementations provided.

### Creating Render Pipeline States with Mesh Shaders

func makeRenderPipelineState(descriptor: MTLMeshRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a mesh render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(descriptor: MTLMeshRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a mesh render pipeline state and reflection information.

**Required** Default implementations provided.

### Creating Tile Render Pipeline States

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption) throws -> (any MTLRenderPipelineState, MTLRenderPipelineReflection?)

Synchronously creates a tile shader’s render pipeline state and reflection information in a tuple.

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedRenderPipelineReflection?>?) throws -> any MTLRenderPipelineState

Synchronously creates a tile shader’s render pipeline state and reflection information.

**Required**

func makeRenderPipelineState(tileDescriptor: MTLTileRenderPipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewRenderPipelineStateWithReflectionCompletionHandler)

Asynchronously creates a tile shader’s render pipeline state and reflection information.

**Required** Default implementation provided.

### Creating Compute Pipeline States

func makeComputePipelineState(descriptor: MTLComputePipelineDescriptor, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedComputePipelineReflection?>?) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state and reflection information.

**Required**

func makeComputePipelineState(descriptor: MTLComputePipelineDescriptor, options: MTLPipelineOption, completionHandler: MTLNewComputePipelineStateWithReflectionCompletionHandler)

Asynchronously creates a compute pipeline state and reflection information.

**Required** Default implementation provided.

func makeComputePipelineState(function: any MTLFunction) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, completionHandler: MTLNewComputePipelineStateCompletionHandler)

Asynchronously creates a compute pipeline state with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, options: MTLPipelineOption, reflection: AutoreleasingUnsafeMutablePointer&lt;MTLAutoreleasedComputePipelineReflection?>?) throws -> any MTLComputePipelineState

Synchronously creates a compute pipeline state and reflection with a function instance.

**Required**

func makeComputePipelineState(function: any MTLFunction, options: MTLPipelineOption, completionHandler: MTLNewComputePipelineStateWithReflectionCompletionHandler)

Asynchronously creates a compute pipeline state and reflection with a function instance.

**Required**

### Creating Depth and Stencil States

func makeDepthStencilState(descriptor: MTLDepthStencilDescriptor) -> (any MTLDepthStencilState)?

Creates a depth-stencil state instance.

**Required**

### Supporting Types

typealias MTLNewRenderPipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline.

typealias MTLNewRenderPipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline and reflection information.

typealias MTLNewComputePipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline.

typealias MTLNewComputePipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline and reflection information.

## See Also

### Working with GPU Devices

Device Inspection

Locate and identify a GPU and the features it supports, and sample its counters.

Work Submission

Create queues that submit work to the GPU or load assets into GPU resources, and indirect command buffers that group your frequent commands together.

Resource Creation

Load assets with input/output queues and make various resource instances, such as buffers, textures, acceleration structures, and memory heaps.

Shader Library and Archive Creation

Create static and dynamic shader libraries, and binary shader archives.

