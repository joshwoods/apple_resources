

- Metal
- Render Passes
- MTLRenderCommandEncoder
-  Render Pass Configuration 

API Collection

# Render Pass Configuration

Set a render pass’s pipeline state, attachment actions, viewports, and so on, that affect subsequent drawing commands.

## Overview

The commands these methods encode configure the render pass for all the subsequent drawing commands (see Render Pass Drawing Commands). The most important part of a render pass’s configuration is its pipeline state (see MTLRenderPipelineState), which you set by calling the setRenderPipelineState(_:) method.

## Topics

### Configuring Pipeline State

func setRenderPipelineState(any MTLRenderPipelineState)

Configures the encoder with a render or tile pipeline state instance that applies to your subsequent draw commands.

**Required**

### Configuring the Actions for Attachments

func setColorStoreAction(MTLStoreAction, index: Int)

Configures the store action for a color attachment.

**Required**

func setColorStoreActionOptions(MTLStoreActionOptions, index: Int)

Configures the store action options for a color attachment.

**Required**

func setDepthStoreAction(MTLStoreAction)

Configures the store action for the depth attachment.

**Required**

func setDepthStoreActionOptions(MTLStoreActionOptions)

Configures the store action options for the depth attachment.

**Required**

func setStencilStoreAction(MTLStoreAction)

Configures the store action for the stencil attachment.

**Required**

func setStencilStoreActionOptions(MTLStoreActionOptions)

Configures the store action options for the stencil attachment.

**Required**

### Configuring Blend Behavior

func setBlendColor(red: Float, green: Float, blue: Float, alpha: Float)

Configures each pixel component value, including alpha, for the render pipeline’s constant blend color.

**Required**

### Configuring Rendering Behavior

func setTriangleFillMode(MTLTriangleFillMode)

Configures how subsequent draw commands rasterize triangle and triangle strip primitives.

**Required**

func setFrontFacing(MTLWinding)

Configures which face of a primitive, such as a triangle, is the front.

**Required**

func setCullMode(MTLCullMode)

Configures how the render pipeline determines which primitives to remove.

**Required**

### Configuring Depth and Stencil Behavior

func setDepthStencilState((any MTLDepthStencilState)?)

Configures the combined depth and stencil state.

**Required**

func setDepthBias(Float, slopeScale: Float, clamp: Float)

Configures the adjustments a render pass applies to depth values from fragment functions by a scaling factor and bias.

**Required**

func setDepthClipMode(MTLDepthClipMode)

Configures how the render pipeline handles fragments outside the near and far planes of the view frustum.

**Required**

func setStencilReferenceValue(UInt32)

Configures the same comparison value for front- and back-facing primitives.

**Required**

func setStencilReferenceValues(front: UInt32, back: UInt32)

Configures different comparison values for front- and back-facing primitives.

**Required**

### Configuring Viewport and Scissor Behavior

func setViewport(MTLViewport)

Configures the render pipeline with a viewport that applies a transformation and a clipping rectangle.

**Required**

func setViewports([MTLViewport])

Configures the render pipeline with multiple viewports that apply transformations and clipping rectangles.

func setScissorRect(MTLScissorRect)

Configures a rectangle for the fragment scissor test.

**Required**

func setScissorRects([MTLScissorRect])

Configures multiple rectangles for the fragment scissor test.

### Configuring Visibility Testing

func setVisibilityResultMode(MTLVisibilityResultMode, offset: Int)

Configures which visibility test the GPU runs and the destination for any results it generates.

**Required**

### Configuring Vertex Amplification

func setVertexAmplificationCount(Int, viewMappings: UnsafePointer&lt;MTLVertexAmplificationViewMapping>?)

Configures the number of output vertices the render pipeline produces for each input vertex, optionally with render target and viewport offsets.

**Required**

### Configuring Tessellation Factors

func setTessellationFactorScale(Float)

Configures the scale factor for per-patch tessellation factors.

**Required**

func setTessellationFactorBuffer((any MTLBuffer)?, offset: Int, instanceStride: Int)

Configures the per-patch tessellation factors for any subsequent patch-drawing commands.

**Required**

### Configuring Persistent Threadgroup Memory

func setObjectThreadgroupMemoryLength(Int, index: Int)

Configures the size of a threadgroup memory buffer for an entry in the object argument table.

**Required**

func setThreadgroupMemoryLength(Int, offset: Int, index: Int)

Configures the size of a threadgroup memory buffer for an entry in the fragment or tile shader argument table.

**Required**

