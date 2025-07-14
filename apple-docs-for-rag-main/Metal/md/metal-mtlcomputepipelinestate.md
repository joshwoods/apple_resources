

- Metal
-  MTLComputePipelineState 

Protocol

# MTLComputePipelineState

An interface that represents a GPU pipeline configuration for running kernels in a compute pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLComputePipelineState : NSObjectProtocol
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

Calculating Threadgroup and Grid Sizes

## Overview

The MTLComputePipelineState protocol is an interface that represents a specific configuration for the GPU pipeline for a compute pass. Use a pipeline state instance to configure a compute pass by calling the setComputePipelineState(_:) method of an MTLComputeCommandEncoder instance.

To create a pipeline state, call the appropriate MTLDevice method (see Pipeline State Creation). You typically make pipeline state instances at a noncritical time, like when your app first launches. This is because graphics drivers may need time to evaluate and build each pipeline state. However, you can quickly use and reuse each pipeline state throughout your app’s lifetime.

## Topics

### Identifying a Pipeline State

var device: any MTLDevice

The device instance that created the pipeline state.

**Required**

var gpuResourceID: MTLResourceID

An unique identifier that represents the pipeline state, which you can add to an argument buffer.

**Required**

var label: String?

A string that helps you identify the compute pipeline state during debugging.

**Required**

### Checking Threadgroup Attributes

var maxTotalThreadsPerThreadgroup: Int

The maximum number of threads in a threadgroup that you can dispatch to the pipeline.

**Required**

var threadExecutionWidth: Int

The number of threads that the GPU executes simultaneously.

**Required**

var staticThreadgroupMemoryLength: Int

The length, in bytes, of statically allocated threadgroup memory.

**Required**

### Checking Imageblock Attributes

func imageblockMemoryLength(forDimensions: MTLSize) -> Int

Returns the length of reserved memory for an imageblock of a given size.

**Required**

### Checking Indirect Command Buffer Support

var supportIndirectCommandBuffers: Bool

A Boolean value that indicates whether the compute pipeline supports indirect command buffers.

**Required**

### Checking Shader Validation

var shaderValidation: MTLShaderValidation

The current state of shader validation for the pipeline.

**Required**

### Creating Function Handles

func functionHandle(function: any MTLFunction) -> (any MTLFunctionHandle)?

Creates a function handle for a visible function.

**Required**

### Adding Visible Functions

func makeComputePipelineStateWithAdditionalBinaryFunctions(functions: [any MTLFunction]) throws -> any MTLComputePipelineState

Creates a new pipeline state object with additional callable functions.

**Required**

### Creating Function Tables

func makeVisibleFunctionTable(descriptor: MTLVisibleFunctionTableDescriptor) -> (any MTLVisibleFunctionTable)?

Creates a new visible function table.

**Required**

func makeIntersectionFunctionTable(descriptor: MTLIntersectionFunctionTableDescriptor) -> (any MTLIntersectionFunctionTable)?

Creates a new intersection function table.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring a Compute Pipeline State

class MTLComputePipelineDescriptor

An instance describing the desired GPU state for a kernel call in a compute pass.

class MTLStageInputOutputDescriptor

A description of the input and output data of a function.

class MTLPipelineBufferDescriptor

The mutability options for a buffer that a render or compute pipeline uses.

class MTLPipelineBufferDescriptorArray

An array of pipeline buffer descriptors.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

