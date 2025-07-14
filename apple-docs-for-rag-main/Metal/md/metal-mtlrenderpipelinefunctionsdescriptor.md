

- Metal
-  MTLRenderPipelineFunctionsDescriptor 

Class

# MTLRenderPipelineFunctionsDescriptor

A collection of functions for updating a render pipeline.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLRenderPipelineFunctionsDescriptor
```

## Overview

When you create a render pipeline that takes visible functions as parameters, you must specify all possible functions that the render pipeline can call. If you already have a pipeline, you can create a new render pipeline with the same configuration but additional callable functions. To create the new pipeline state object, configure a MTLRenderPipelineFunctionsDescriptor object with the additional callable functions to add, and then call the pipeline state object’s makeRenderPipelineState(additionalBinaryFunctions:) method, passing the descriptor.

## Topics

### Configuring the Descriptor’s Functions

var vertexAdditionalBinaryFunctions: [any MTLFunction]?

The vertex functions to add to the render pipeline.

var fragmentAdditionalBinaryFunctions: [any MTLFunction]?

The fragment functions to add to the render pipeline.

var tileAdditionalBinaryFunctions: [any MTLFunction]?

The tile functions to add to the render pipeline.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Render Pipeline States

protocol MTLRenderPipelineState

An interface that represents a graphics pipeline configuration for a render pass, which the pass applies to the draw commands you encode.

class MTLRenderPipelineDescriptor

An argument of options you pass to a GPU device to get a render pipeline state.

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

