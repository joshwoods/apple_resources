

- Metal
-  MTLRenderPipelineState 

Protocol

# MTLRenderPipelineState

An interface that represents a graphics pipeline configuration for a render pass, which the pass applies to the draw commands you encode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLRenderPipelineState : NSObjectProtocol
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

Improving Rendering Performance with Vertex Amplification

## Overview

The MTLRenderPipelineState protocol is an interface that represents a specific configuration for the graphics-rendering pipeline, including which shaders it uses. Use a pipeline state instance to configure a render pass by calling the setRenderPipelineState(_:) method of an MTLRenderCommandEncoder instance.

To create a pipeline state, call the appropriate MTLDevice method (see Pipeline State Creation). You typically make pipeline state instances at a noncritical time, like when the app first launches. This is because graphics drivers may need time to evaluate and build each pipeline state. However, you can quickly use and reuse each pipeline state throughout your app’s lifetime.

## Topics

### Identifying a Pipeline State

var device: any MTLDevice

The device instance that creates the pipeline state.

**Required**

var label: String?

A string that helps you identify the render pipeline state during debugging.

**Required**

var gpuResourceID: MTLResourceID

An unique identifier that represents the pipeline state, which you can add to an argument buffer.

**Required**

### Checking Object Shader Memory Requirements

var maxTotalThreadsPerObjectThreadgroup: Int

The largest number of threads the pipeline state can have in a single object shader threadgroup.

**Required**

var objectThreadExecutionWidth: Int

The number of threads the render pass applies to a SIMD group for an object shader.

**Required**

### Checking Mesh Shader Memory Requirements

var maxTotalThreadsPerMeshThreadgroup: Int

The largest number of threads the pipeline state can have in a single mesh shader threadgroup.

**Required**

var maxTotalThreadgroupsPerMeshGrid: Int

The largest number of threadgroups the pipeline state can have in a single mesh shader grid.

**Required**

var meshThreadExecutionWidth: Int

The number of threads the render pass applies to a SIMD group for a mesh shader.

**Required**

### Checking Tile Shader Memory Requirements

var maxTotalThreadsPerThreadgroup: Int

The largest number of threads the pipeline state can have in a single tile shader threadgroup.

**Required**

var threadgroupSizeMatchesTileSize: Bool

A Boolean value that indicates whether the pipeline state needs a threadgroup’s size to equal a tile’s size.

**Required**

var imageblockSampleLength: Int

The memory size, in byes, of the render pipeline’s imageblock for a single sample.

**Required**

func imageblockMemoryLength(forDimensions: MTLSize) -> Int

Returns the length of an imageblock’s memory for the specified imageblock dimensions.

**Required**

### Checking Feature Support

var supportIndirectCommandBuffers: Bool

A Boolean value that indicates whether the render pipeline supports encoding commands into an indirect command buffer.

**Required**

### Checking Shader Validation

var shaderValidation: MTLShaderValidation

The current state of shader validation for the pipeline.

**Required**

### Creating Function Handles and Tables

func functionHandle(function: any MTLFunction, stage: MTLRenderStages) -> (any MTLFunctionHandle)?

Creates a function handle for a shader.

**Required**

func makeVisibleFunctionTable(descriptor: MTLVisibleFunctionTableDescriptor, stage: MTLRenderStages) -> (any MTLVisibleFunctionTable)?

Creates a new visible function table.

**Required**

func makeIntersectionFunctionTable(descriptor: MTLIntersectionFunctionTableDescriptor, stage: MTLRenderStages) -> (any MTLIntersectionFunctionTable)?

Creates a new intersection function table.

**Required**

### Creating Modified Clones of the Render Pipeline

func makeRenderPipelineState(additionalBinaryFunctions: MTLRenderPipelineFunctionsDescriptor) throws -> any MTLRenderPipelineState

Creates a new pipeline state that’s a copy of the current pipeline state with additional shaders.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Render Pipeline States

class MTLRenderPipelineDescriptor

An argument of options you pass to a GPU device to get a render pipeline state.

class MTLRenderPipelineFunctionsDescriptor

A collection of functions for updating a render pipeline.

class MTLMeshRenderPipelineDescriptor

An object that configures new render pipeline state objects for mesh shading.

class MTLPipelineBufferDescriptor

The mutability options for a buffer that a render or compute pipeline uses.

class MTLPipelineBufferDescriptorArray

An array of pipeline buffer descriptors.

class MTLRenderPipelineColorAttachmentDescriptor

A color render target that specifies the color configuration and color operations for a render pipeline.

class MTLRenderPipelineColorAttachmentDescriptorArray

An array of render pipeline color attachment descriptor objects.

class MTLTileRenderPipelineDescriptor

An object that configures new render pipeline state objects for tile shading.

class MTLTileRenderPipelineColorAttachmentDescriptor

A description of a tile-shading render pipeline’s color render target.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

