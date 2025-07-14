

- Metal
-  MTLTileRenderPipelineDescriptor 

Class

# MTLTileRenderPipelineDescriptor

An object that configures new render pipeline state objects for tile shading.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
class MTLTileRenderPipelineDescriptor
```

## Topics

### Identifying the Render Pipeline

var label: String?

A string that identifies the tile pipeline descriptor.

### Specifying Graphics Functions and Associated Data

var tileFunction: any MTLFunction

The compute kernel or fragment function the pipeline calls.

var tileBuffers: MTLPipelineBufferDescriptorArray

An array that contains the buffer mutability options for a render pipeline’s tile function.

var maxCallStackDepth: Int

The maximum function call depth from the top-most shader function.

### Specifying Rasterization and Visibility State

var threadgroupSizeMatchesTileSize: Bool

A Boolean value that indicates whether all threadgroups for this pipeline completely cover tiles.

var rasterSampleCount: Int

The number of samples in each fragment.

### Specifying Rendering Pipeline State

func reset()

Specifies the default rendering pipeline state values for the descriptor.

var colorAttachments: MTLTileRenderPipelineColorAttachmentDescriptorArray

An array of attachments that store color data.

### Specifying Threads per Threadgroup

var maxTotalThreadsPerThreadgroup: Int

The maximum number of threads in a threadgroup when dispatching a command using the pipeline.

### Specifying Precompiled Shader Binaries

var supportAddingBinaryFunctions: Bool

A Boolean value that indicates whether you can use the pipeline to create new pipelines by adding binary functions to its callable functions list.

var binaryArchives: [any MTLBinaryArchive]?

An array of binary archives to search for precompiled versions of the shader.

### Specifying Callable Functions for the Pipeline

var linkedFunctions: MTLLinkedFunctions!

Functions that you can specify as function arguments for the tile shader when encoding commands that use the pipeline.

### Specifying Shader Validation

var shaderValidation: MTLShaderValidation

A value that enables or disables shader validation for the pipeline.

### Instance Properties

var preloadedLibraries: [any MTLDynamicLibrary]

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

class MTLTileRenderPipelineColorAttachmentDescriptor

A description of a tile-shading render pipeline’s color render target.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

