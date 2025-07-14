

- Metal
- Render Passes
- MTLRenderCommandEncoder
-  Render Pass Drawing Commands 

API Collection

# Render Pass Drawing Commands

Render an image by drawing meshes, primitives, tessellation patches, and by dispatching tile shaders.

## Overview

The drawing commands these methods encode inherit the encoder’s current state for the render pass (see Render Pass Configuration), including resource assignments. For more information about preparing resources for your drawing commands, see Vertex Shader Resource Preparation Commands, Argument Buffer Resource Preparation Commands, and their sibling pages.

To render tessellated patches, configure the render pass with a post-tessellation vertex shader.

Important

Post-tessellation vertex shaders only apply to the tessellation patch-drawing methods.

## Topics

### Drawing with Meshes

func drawMeshThreads(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threads.

**Required**

func drawMeshThreadgroups(MTLSize, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with a grid of threadgroups.

**Required**

func drawMeshThreadgroups(indirectBuffer: any MTLBuffer, indirectBufferOffset: Int, threadsPerObjectThreadgroup: MTLSize, threadsPerMeshThreadgroup: MTLSize)

Encodes a draw command that invokes a mesh shader and, optionally, an object shader with indirect arguments.

**Required**

### Drawing with Vertices

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int)

Encodes a draw command that renders an instance of a geometric primitive.

**Required**

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int, instanceCount: Int)

Encodes a draw command that renders multiple instances of a geometric primitive.

**Required**

func drawPrimitives(type: MTLPrimitiveType, vertexStart: Int, vertexCount: Int, instanceCount: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of a geometric primitive that starts with a custom instance identification number.

**Required**

func drawPrimitives(type: MTLPrimitiveType, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indirect arguments.

**Required**

### Drawing with Indexed Vertices

func drawIndexedPrimitives(type: MTLPrimitiveType, indexCount: Int, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int)

Encodes a draw command that renders an instance of a geometric primitive with indexed vertices.

**Required**

func drawIndexedPrimitives(type: MTLPrimitiveType, indexCount: Int, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int, instanceCount: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices.

**Required**

func drawIndexedPrimitives(type: MTLPrimitiveType, indexCount: Int, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int, instanceCount: Int, baseVertex: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices, starting with a custom vertex and instance.

**Required**

func drawIndexedPrimitives(type: MTLPrimitiveType, indexType: MTLIndexType, indexBuffer: any MTLBuffer, indexBufferOffset: Int, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of a geometric primitive with indexed vertices and indirect arguments.

**Required**

### Drawing with Tessellation Patches

func drawPatches(numberOfPatchControlPoints: Int, patchStart: Int, patchCount: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, instanceCount: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of tessellated patches.

**Required**

func drawPatches(numberOfPatchControlPoints: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of tessellated patches with indirect arguments.

**Required**

### Drawing with Indexed Tessellation Patches

func drawIndexedPatches(numberOfPatchControlPoints: Int, patchStart: Int, patchCount: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, controlPointIndexBuffer: any MTLBuffer, controlPointIndexBufferOffset: Int, instanceCount: Int, baseInstance: Int)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer.

**Required**

func drawIndexedPatches(numberOfPatchControlPoints: Int, patchIndexBuffer: (any MTLBuffer)?, patchIndexBufferOffset: Int, controlPointIndexBuffer: any MTLBuffer, controlPointIndexBufferOffset: Int, indirectBuffer: any MTLBuffer, indirectBufferOffset: Int)

Encodes a draw command that renders multiple instances of tessellated patches with a control point index buffer and indirect arguments.

**Required**

### Drawing with Tile Shaders

func dispatchThreadsPerTile(MTLSize)

Encodes a command that invokes GPU functions from the encoder’s current tile render pipeline state.

**Required**

var tileWidth: Int

The width of the tiles, in pixels, for the render command encoder.

**Required**

var tileHeight: Int

The height of the tiles, in pixels, for the render command encoder.

**Required**

