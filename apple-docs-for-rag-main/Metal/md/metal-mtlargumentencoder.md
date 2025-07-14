

- Metal
-  MTLArgumentEncoder 

Protocol

# MTLArgumentEncoder

An object used to encode data into an argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol MTLArgumentEncoder : NSObjectProtocol
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Overview

A MTLArgumentEncoder object encodes buffers, textures, samplers, and inlined constant data into an argument buffer. A MTLBuffer object represents the argument buffer that you set as the encoding destination by calling the setArgumentBuffer(_:offset:) method.

The recommended way to declare an argument buffer is to define its structure in your Metal shading language code. You can assign the argument buffer to a function’s specific buffer index. To create an encoder for this type of argument buffer, call one of the following MTLFunction methods:

- makeArgumentEncoder(bufferIndex:)

- makeArgumentEncoder(bufferIndex:reflection:)

If you construct your shaders dynamically at runtime, you can still construct argument buffers as parameters for the shader. Define each argument separately and then add it to an array of MTLArgumentDescriptor objects. To create an encoder for this type of argument buffer, call the makeArgumentEncoder(arguments:) method of the MTLDevice class.

Important

A runtime validation error occurs if you create a `MTLArgumentEncoder` object using structures that don’t reference any other resources and don’t provide any `[[id()]]` annotation on any of their members.

## Topics

### Creating an Argument Buffer

func setArgumentBuffer((any MTLBuffer)?, offset: Int)

Specifies the position in a buffer where the encoder writes argument data.

**Required**

func setArgumentBuffer((any MTLBuffer)?, startOffset: Int, arrayElement: Int)

Specifies an array element within a buffer where the encoder writes argument data.

**Required**

var encodedLength: Int

The number of bytes required to store the encoded resources of an argument buffer.

**Required**

### Encoding Buffers

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Encodes a reference to a buffer into the argument buffer.

**Required**

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Encodes references to an array of buffers into the argument buffer.

### Encoding Textures

func setTexture((any MTLTexture)?, index: Int)

Encodes a reference to a texture into the argument buffer.

**Required**

func setTextures([(any MTLTexture)?], range: Range&lt;Int>)

Encodes references to an array of textures into the argument buffer.

### Encoding Samplers

func setSamplerState((any MTLSamplerState)?, index: Int)

Encodes a sampler into the argument buffer.

**Required**

func setSamplerStates([(any MTLSamplerState)?], range: Range&lt;Int>)

Encodes an array of samplers into the argument buffer.

### Encoding Pipeline States

func setRenderPipelineState((any MTLRenderPipelineState)?, index: Int)

Encodes a reference to a render pipeline state into the argument buffer.

**Required**

func setRenderPipelineStates([(any MTLRenderPipelineState)?], range: Range&lt;Int>)

Encodes references to an array of render pipeline states into the argument buffer.

func setComputePipelineState((any MTLComputePipelineState)?, index: Int)

Encodes a reference to a compute pipeline state into the argument buffer.

**Required**

func setComputePipelineStates(UnsafePointer&lt;(any MTLComputePipelineState)?>, with: NSRange)

Encodes references to an array of compute pipeline states into the argument buffer.

func setComputePipelineState((any MTLComputePipelineState)?, at: Int)

Encodes a reference to a compute pipeline state into the argument buffer.

func setComputePipelineStates([(any MTLComputePipelineState)?], range: Range&lt;Int>)

Encodes references to an array of compute pipeline states into the argument buffer.

### Encoding Inlined Constant Data

func constantData(at: Int) -> UnsafeMutableRawPointer

Returns a pointer to an inline, constant-data argument within the argument buffer.

**Required**

### Encoding Indirect Command Buffers

func setIndirectCommandBuffer((any MTLIndirectCommandBuffer)?, index: Int)

Encodes a reference to an indirect command buffer into the argument buffer.

**Required**

func setIndirectCommandBuffers([(any MTLIndirectCommandBuffer)?], range: Range&lt;Int>)

Encodes an array of indirect command buffers into the argument buffer.

### Encoding Acceleration Structures

func setAccelerationStructure((any MTLAccelerationStructure)?, index: Int)

Encodes a reference to an acceleration structure into the argument buffer.

**Required**

### Encoding Function Tables

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, index: Int)

Encodes a reference to a visible-function table into the argument buffer.

**Required**

func setIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, index: Int)

Encodes a reference to a ray-tracing intersection-function table into the argument buffer.

**Required**

func setIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], range: Range&lt;Int>)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], range: Range&lt;Int>)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

### Creating a Nested Argument Encoder

func makeArgumentEncoderForBuffer(atIndex: Int) -> (any MTLArgumentEncoder)?

Creates a new argument encoder for a nested argument buffer.

**Required**

### Querying Alignment

var alignment: Int

The alignment, in bytes, required for storing the encoded resources of an argument buffer.

**Required**

### Identifying the Argument Encoder

var label: String?

A string that identifies the argument buffer.

**Required**

var device: any MTLDevice

The device object that created the argument encoder.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Argument Buffers

Improving CPU Performance by Using Argument Buffers

Optimize your app’s performance by grouping your resources into argument buffers.

Managing groups of resources with argument buffers

Create argument buffers to organize related resources.

Tracking the Resource Residency of Argument Buffers

Optimize resource performance within an argument buffer.

Indexing Argument Buffers

Assign resource indices within an argument buffer.

Rendering Terrain Dynamically with Argument Buffers

Use argument buffers to render terrain in real time with a GPU-driven pipeline.

Encoding Argument Buffers on the GPU

Use a compute pass to encode an argument buffer and access its arguments in a subsequent render pass.

Using Argument Buffers with Resource Heaps

Reduce CPU overhead by using arrays inside argument buffers and combining them with resource heaps.

class MTLArgumentDescriptor

A representation of an argument within an argument buffer.

let MTLAttributeStrideStatic: Int

