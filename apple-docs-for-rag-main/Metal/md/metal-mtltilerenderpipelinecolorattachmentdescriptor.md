

- Metal
-  MTLTileRenderPipelineColorAttachmentDescriptor 

Class

# MTLTileRenderPipelineColorAttachmentDescriptor

A description of a tile-shading render pipeline’s color render target.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
class MTLTileRenderPipelineColorAttachmentDescriptor
```

## Topics

### Specifying Pixel Format

var pixelFormat: MTLPixelFormat

The pixel format associated with the tile shading render pipeline.

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

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

