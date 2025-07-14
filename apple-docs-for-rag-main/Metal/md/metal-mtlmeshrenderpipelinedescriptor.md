

- Metal
-  MTLMeshRenderPipelineDescriptor 

Class

# MTLMeshRenderPipelineDescriptor

An object that configures new render pipeline state objects for mesh shading.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLMeshRenderPipelineDescriptor
```

## Topics

### Instance Properties

var binaryArchives: [any MTLBinaryArchive]?

var colorAttachments: MTLRenderPipelineColorAttachmentDescriptorArray

var depthAttachmentPixelFormat: MTLPixelFormat

var fragmentBuffers: MTLPipelineBufferDescriptorArray

var fragmentFunction: (any MTLFunction)?

var fragmentLinkedFunctions: MTLLinkedFunctions!

var isAlphaToCoverageEnabled: Bool

var isAlphaToOneEnabled: Bool

var isRasterizationEnabled: Bool

var label: String?

var maxTotalThreadgroupsPerMeshGrid: Int

var maxTotalThreadsPerMeshThreadgroup: Int

var maxTotalThreadsPerObjectThreadgroup: Int

var maxVertexAmplificationCount: Int

var meshBuffers: MTLPipelineBufferDescriptorArray

var meshFunction: (any MTLFunction)?

var meshLinkedFunctions: MTLLinkedFunctions!

var meshThreadgroupSizeIsMultipleOfThreadExecutionWidth: Bool

var objectBuffers: MTLPipelineBufferDescriptorArray

var objectFunction: (any MTLFunction)?

var objectLinkedFunctions: MTLLinkedFunctions!

var objectThreadgroupSizeIsMultipleOfThreadExecutionWidth: Bool

var payloadMemoryLength: Int

var rasterSampleCount: Int

var shaderValidation: MTLShaderValidation

A value that enables or disables shader validation for the pipeline.

var stencilAttachmentPixelFormat: MTLPixelFormat

var supportIndirectCommandBuffers: Bool

### Instance Methods

func reset()

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

