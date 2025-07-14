

- Metal
-  MTLIndirectRenderCommand 

Protocol

# MTLIndirectRenderCommand

A render command in an indirect command buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
protocol MTLIndirectRenderCommand : NSObjectProtocol
```

## Overview

Don’t implement this protocol; you get objects of this type by asking a MTLIndirectCommandBuffer for them.

Use this object to reset or encode a command. You must always reset a command before encoding a new command.

## Topics

### Setting Command Arguments

func setRenderPipelineState(any MTLRenderPipelineState)

Sets the render pipeline state object used by the command.

**Required**

func setVertexBuffer(any MTLBuffer, offset: Int, at: Int)

Sets a vertex buffer argument for the command.

**Required**

func setFragmentBuffer(any MTLBuffer, offset: Int, at: Int)

Sets a fragment buffer argument for the command.

**Required**

### Encoding a Drawing Command

func drawPrimitives(MTLPrimitiveType, vertexStart: Int, vertexCount: Int, instanceCount: Int, baseInstance: Int)

Encodes a command to render a number of instances of primitives using vertex data in contiguous array elements, starting from the base instance.

**Required**

func drawIndexedPrimitives(MTLPrimitiveType, indexCount: Int, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int, instanceCount: Int, baseVertex: Int, baseInstance: Int)

Encodes a command to render a number of instances of primitives using an index list specified in a buffer, starting from the base vertex of the base instance.

**Required**

func drawPatches(Int, patchStart: Int, patchCount: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, instanceCount: Int, baseInstance: Int, tessellationFactorBuffer: any MTLBuffer, tessellationFactorBufferOffset: Int, tessellationFactorBufferInstanceStride: Int)

Encodes a command to render a number of instances of tessellated patches.

**Required**

func drawIndexedPatches(Int, patchStart: Int, patchCount: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, controlPointIndexBuffer: any MTLBuffer, controlPointIndexBufferOffset: Int, instanceCount: Int, baseInstance: Int, tessellationFactorBuffer: any MTLBuffer, tessellationFactorBufferOffset: Int, tessellationFactorBufferInstanceStride: Int)

Encodes a command to render a number of instances of tessellated patches, using a control point index buffer.

**Required**

### Resetting a Command

func reset()

Resets the command to its default state.

**Required**

### Instance Methods

func clearBarrier()

**Required**

func drawMeshThreadgroups(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

**Required**

func drawMeshThreads(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

**Required**

func setBarrier()

**Required**

func setMeshBuffer(any MTLBuffer, offset: Int, at: Int)

**Required**

func setObjectBuffer(any MTLBuffer, offset: Int, at: Int)

**Required**

func setObjectThreadgroupMemoryLength(Int, index: Int)

**Required**

func setVertexBuffer(any MTLBuffer, offset: Int, attributeStride: Int, at: Int)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Render Compute Commands

struct MTLDrawPatchIndirectArguments

The data layout required for drawing patches via indirect buffer calls.

struct MTLDrawPrimitivesIndirectArguments

The data layout required for drawing primitives via indirect buffer calls.

struct MTLDrawIndexedPrimitivesIndirectArguments

The data layout required for drawing indexed primitives via indirect buffer calls.

