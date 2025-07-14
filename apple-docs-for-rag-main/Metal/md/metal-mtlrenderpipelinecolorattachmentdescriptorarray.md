

- Metal
-  MTLRenderPipelineColorAttachmentDescriptorArray 

Class

# MTLRenderPipelineColorAttachmentDescriptorArray

An array of render pipeline color attachment descriptor objects.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLRenderPipelineColorAttachmentDescriptorArray
```

## Topics

### Accessing Render Pipeline State for a Color Attachment

subscript(Int) -> MTLRenderPipelineColorAttachmentDescriptor!

Returns the render pipeline state for the specified color attachment.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Render Pipeline States

protocol MTLRenderPipelineState

An interface that represents a graphics pipeline configuration for a render pass, which the pass applies to the draw commands you encode.

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

class MTLTileRenderPipelineDescriptor

An object that configures new render pipeline state objects for tile shading.

class MTLTileRenderPipelineColorAttachmentDescriptor

A description of a tile-shading render pipeline’s color render target.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

