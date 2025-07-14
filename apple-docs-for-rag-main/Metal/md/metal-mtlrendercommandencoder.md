

- Metal
-  MTLRenderCommandEncoder 

Protocol

# MTLRenderCommandEncoder

An interface that encodes a render pass into a command buffer, including all its draw calls and configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
protocol MTLRenderCommandEncoder : MTLCommandEncoder
```

## Mentioned in 

Improving Rendering Performance with Vertex Amplification

Improving CPU Performance by Using Argument Buffers

Setting Up a Command Structure

Sampling GPU Data into Counter Sample Buffers

Tracking the Resource Residency of Argument Buffers

## Overview

The MTLRenderCommandEncoder protocol defines an interface that configures and encodes a render pass. Use a render pass to draw a scene, or a component within a scene, to its render *attachments*, the outputs of a render pass. You can use various approaches to render to those outputs, including techniques that apply the following:

- Primitive drawing

- Mesh drawing

- Ray tracing

- Tile shaders dispatching

To create an MTLRenderCommandEncoder instance, call the makeRenderCommandEncoder(descriptor:) of an MTLCommandBuffer instance, or the makeRenderCommandEncoder() method of an MTLParallelRenderCommandEncoder instance.

To configure the render pass for your first drawing commands, start with a pipeline state by passing an MTLRenderPipelineState instance to the encoder’s setRenderPipelineState(_:) method. You create the pipeline states your render pass needs, typically ahead of time, by calling one or more MTLDevice methods (see Pipeline State Creation).

Tip

Avoid visual stutter by creating pipeline states at a noncritical time, such as during launch, because of the time it can take to make them.

Set any other applicable parts of the encoder’s configuration by calling the methods on the Render Pass Configuration page. For example, you may need to configure the pass’s viewport, its scissor rectangle, and the settings for depth and stencil tests.

Assign resources, such as buffers and textures, for the shaders that depend on them. For more information, see the shader-specific pages in the resource preparation section, such as Vertex Shader Resource Preparation Commands and Fragment Shader Resource Preparation Commands. If your shaders access resources through an argument buffer, ensure the pass makes those resources *resident* by loading those resources resident in GPU memory. You do this by calling the methods on the Argument Buffer Resource Preparation Commands page.

Encode drawing commands by calling the methods on the Render Pass Drawing Commands page after you configure the state and resources the commands depend on. The encoder maintains its current state and applies them to all subsequent draw commands. For drawing commands that need different states or resources, reconfigure the render pass appropriately and then encode those draw commands. Repeat the process for each batch of drawing commands that depend on the same render pass configuration and resources.

When you finish encoding the render pass’s commands, finalize it into the command buffer by calling the encoder’s endEncoding() method.

## Topics

### Encoding Configuration Commands

Manage the render pass’s overall state.

Render Pass Configuration

Set a render pass’s pipeline state, attachment actions, viewports, and so on, that affect subsequent drawing commands.

### Encoding Resource Preparation Commands

Load buffers, textures, and other resources into GPU memory for each shader type, including mesh, object, vertex, fragment, and tile shaders.

Mesh and Object Shader Resource Preparation Commands

Assign resources to mesh and object shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Vertex Shader Resource Preparation Commands

Assign resources to vertex shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Fragment Shader Resource Preparation Commands

Assign resources to fragment shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Tile Shaders Resource Preparation Commands

Assign resources to tile shaders, including buffers, textures, acceleration structures, sampler states, and function tables.

Argument Buffer Resource Preparation Commands

Load individual resources and multiple resources within a heap into GPU memory so that they’re available to shaders through argument buffers.

### Encoding Draw Commands

Render your content with draw commands that invoke the shaders of the pass’s current pipeline state.

Render Pass Drawing Commands

Render an image by drawing meshes, primitives, tessellation patches, and by dispatching tile shaders.

### Encoding Resource Synchronization Commands

Protect against data hazards for resources with a hazardTrackingMode property that’s MTLHazardTrackingMode.untracked with memory fences and barriers.

func waitForFence(any MTLFence, before: MTLRenderStages)

Encodes a command that instructs the GPU to pause before starting one or more stages of the render pass until a pass updates a fence.

**Required**

func updateFence(any MTLFence, after: MTLRenderStages)

Encodes a command that instructs the GPU to update a fence after one or more stages, which signals passes waiting on the fence.

**Required**

func memoryBarrier(resources: [any MTLResource], after: MTLRenderStages, before: MTLRenderStages)

Creates a memory barrier that enforces the order of write and read operations for specific resources.

func memoryBarrier(scope: MTLBarrierScope, after: MTLRenderStages, before: MTLRenderStages)

Creates a memory barrier that enforces the order of write and read operations for specific resource types.

**Required**

### Encoding Commands that Run Indirect Command Buffers

Run a command that tells the GPU to run other commands in a buffer, typically for commands your app needs frequently.

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, range: Range&lt;Int>)

Encodes a command that runs a range of commands from an indirect command buffer (ICB).

func executeCommandsInBuffer(any MTLIndirectCommandBuffer, indirectBuffer: any MTLBuffer, offset: Int)

Encodes a command that runs an indirect range of commands from an indirect command buffer (ICB).

### Encoding Data Sampling Commands

Sample realtime data from the GPU’s hardware as it runs the render pass.

func sampleCounters(sampleBuffer: any MTLCounterSampleBuffer, sampleIndex: Int, barrier: Bool)

Encodes a command that samples hardware counters during the render pass and stores the data into a counter sample buffer.

**Required**

### Deprecated

Replace older symbols in this group with their newer equivalents.

Deprecated Symbols

Review unsupported symbols and their replacements.

### Instance Methods

func setVertexBuffer((any MTLBuffer)?, offset: Int, attributeStride: Int, index: Int)

**Required**

func setVertexBufferOffset(offset: Int, attributeStride: Int, index: Int)

**Required**

func setVertexBuffers([(any MTLBuffer)?], offsets: [Int], attributeStrides: [Int], range: Range&lt;Int>)

func setVertexBytes(UnsafeRawPointer, length: Int, attributeStride: Int, index: Int)

**Required**

## Relationships

### Inherits From

- MTLCommandEncoder
- NSObjectProtocol

## See Also

### Encoding a Render Pass

enum MTLTriangleFillMode

Specifies how to rasterize triangle and triangle strip primitives.

enum MTLWinding

The vertex winding rule that determines a front-facing primitive.

enum MTLCullMode

The mode that determines whether to perform culling and which type of primitive to cull.

enum MTLPrimitiveType

The geometric primitive type for drawing commands.

enum MTLIndexType

The index type for an index buffer that references vertices of geometric primitives.

enum MTLDepthClipMode

The mode that determines how to deal with fragments outside of the near or far planes.

enum MTLVisibilityResultMode

The mode that determines what, if anything, the GPU writes to the results buffer, after the GPU executes the render pass.

