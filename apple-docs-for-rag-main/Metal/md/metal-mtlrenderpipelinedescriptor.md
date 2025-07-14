

- Metal
-  MTLRenderPipelineDescriptor 

Class

# MTLRenderPipelineDescriptor

An argument of options you pass to a GPU device to get a render pipeline state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLRenderPipelineDescriptor
```

## Mentioned in 

Rendering to Multiple Texture Slices in a Draw Command

Compiling Binary Archives from a Custom Configuration Script

Creating Binary Archives from Device-Built Pipeline State Objects

Improving Rendering Performance with Vertex Amplification

## Overview

An MTLRenderPipelineDescriptor instance configures the state of the pipeline to use during a rendering pass, including rasterization (such as multisampling), visibility, blending, tessellation, and graphics function state. Use standard allocation and initialization techniques to create an MTLRenderPipelineDescriptor object. Then configure and use the descriptor to create an MTLRenderPipelineState object.

To specify the vertex or fragment function in the rendering pipeline descriptor, set the vertexFunction or fragmentFunction property, respectively, to the desired MTLFunction object. The system ignores the tessellation stage properties if you don’t set the vertexFunction property to a post-tessellation vertex function. A vertex function is a post-tessellation vertex function if the `[[ patch(patch-type, N) ]]` attribute precedes the function’s signature in your Metal Shading Language source. See the “Post-Tessellation Vertex Functions” section of Metal Shading Language Specification for more information.

Setting the fragmentFunction property to `nil` disables the rasterization of pixels into the color attachment. This action is typically for outputting vertex function data into a buffer object, or for depth-only rendering.

If the vertex shader has an argument with per-vertex input attributes, set the vertexDescriptor property to an MTLVertexDescriptor object that describes the organization of that vertex data.

### Multisampling and the Render Pipeline

If a color attachment supports multisampling (essentially, the attachment is an MTLTextureType.type2DMultisample type color texture), you can create multiple samples per fragment, and the following rendering pipeline descriptor properties determine coverage:

- rasterSampleCount is the number of samples for each pixel.

- If isAlphaToCoverageEnabled is true, the GPU uses the alpha channel fragment output for colorAttachments to compute a coverage mask that affects the values the GPU writes to all attachments (color, depth, and stencil).

- If isAlphaToOneEnabled is true, the GPU changes alpha channel fragment values for colorAttachments to `1.0`, which is the largest representable value.

If isAlphaToCoverageEnabled is true, an implementation-defined `coverageToMask` function uses the alpha channel fragment output from colorAttachments to create an intermediate coverage mask, which sets a number of bits in its output proportionally to the value of the floating-point input. For example, if the input is `0.0f`, the function sets the output to `0x0`. If the input is `1.0f`, the function sets all output bits (in effect, `~0x0`). If the input is `0.5f`, the function sets half of the bits, according to the implementation, which often uses dither patterns.

To determine a final coverage mask, the function performs a logical `AND` on the resulting coverage mask `alphaCoverageMask` with the masks from the rasterizer and fragment shader, as the following code shows:

```
if (alphaToCoverageEnabled) then
    alphaCoverageMask = coverageToMask(colorAttachment0.alpha);

finalCoverageMask = originalRasterizerCoverageMask
                    & alphaCoverageMask
                    & fragShaderSampleMaskOutput;
```

## Topics

### Identifying the Render Pipeline State Object

var label: String?

A string that identifies the render pipeline descriptor.

### Specifying Graphics Functions and Associated Data

var vertexFunction: (any MTLFunction)?

The vertex function the pipeline calls to process vertices.

var fragmentFunction: (any MTLFunction)?

The fragment function the pipeline calls to process fragments.

var maxVertexCallStackDepth: Int

The maximum function call depth from the top-most vertex shader function.

var maxFragmentCallStackDepth: Int

The maximum function call depth from the top-most fragment shader function.

### Specifying Buffer Layouts and Fetch Behavior

var vertexDescriptor: MTLVertexDescriptor?

The organization of vertex data in an attribute’s argument table.

### Specifying Buffer Mutability

var vertexBuffers: MTLPipelineBufferDescriptorArray

An array that contains the buffer mutability options for a render pipeline’s vertex function.

var fragmentBuffers: MTLPipelineBufferDescriptorArray

An array that contains the buffer mutability options for a render pipeline’s fragment function.

### Specifying Rendering Pipeline State

func reset()

Specifies the default rendering pipeline state values for the descriptor.

var colorAttachments: MTLRenderPipelineColorAttachmentDescriptorArray

An array of attachments that store color data.

var depthAttachmentPixelFormat: MTLPixelFormat

The pixel format of the attachment that stores depth data.

var stencilAttachmentPixelFormat: MTLPixelFormat

The pixel format of the attachment that stores stencil data.

### Specifying Rasterization and Visibility State

var isAlphaToCoverageEnabled: Bool

A Boolean value that indicates whether to read and use the alpha channel fragment output for color attachments to compute a sample coverage mask.

var isAlphaToOneEnabled: Bool

A Boolean value that indicates whether to force alpha channel values for color attachments to the largest representable value.

var isRasterizationEnabled: Bool

A Boolean value that determines whether the pipeline rasterizes primitives.

var inputPrimitiveTopology: MTLPrimitiveTopologyClass

The type of primitive topology the pipeline renders.

var rasterSampleCount: Int

The number of samples the pipeline applies for each fragment.

enum MTLPrimitiveTopologyClass

The primitive topologies available for rendering.

var sampleCount: Int

The number of samples the pipeline applies for each fragment.

Deprecated

### Specifying Tessellation State

var maxTessellationFactor: Int

The maximum tessellation factor that the tessellator uses when tessellating patches.

var isTessellationFactorScaleEnabled: Bool

A Boolean value that determines whether the pipeline scales the tessellation factor.

var tessellationFactorFormat: MTLTessellationFactorFormat

The format of the tessellation factors in the tessellation factor buffer.

var tessellationControlPointIndexType: MTLTessellationControlPointIndexType

The size of the control point indices in a control point index buffer.

var tessellationFactorStepFunction: MTLTessellationFactorStepFunction

The step function for determining the tessellation factors for a patch from the tessellation factor buffer.

var tessellationOutputWindingOrder: MTLWinding

The winding order of triangles from the tessellator.

var tessellationPartitionMode: MTLTessellationPartitionMode

The partitioning mode that the tessellator uses to derive the number and spacing of segments for subdividing a corresponding edge.

enum MTLTessellationFactorFormat

Options for specifying the format of the tessellation factors in a tessellation factor buffer.

enum MTLTessellationControlPointIndexType

Options for specifying the size of the control point indices in a control point index buffer.

enum MTLTessellationFactorStepFunction

Options for specifying the step function that determines the tessellation factors for a patch from the tessellation factor buffer.

enum MTLTessellationPartitionMode

Options for choosing the partition mode that the tessellator applies when deriving the number and spacing of segments for subdividing a corresponding edge.

### Specifying Indirect Command Buffers Usage

var supportIndirectCommandBuffers: Bool

A Boolean value that determines whether you can encode commands into an indirect command buffer using the render pipeline.

### Specifying the Maximum Vertex Amplification Count

var maxVertexAmplificationCount: Int

The maximum vertex amplification count you can set when encoding render commands.

### Specifying Precompiled Shader Binaries

var supportAddingVertexBinaryFunctions: Bool

A Boolean value that indicates whether you can use the pipeline to create new pipelines by adding binary functions to the vertex shader’s callable functions list.

var supportAddingFragmentBinaryFunctions: Bool

A Boolean value that indicates whether you can use the pipeline to create new pipelines by adding binary functions to the fragment shader’s callable functions list.

var binaryArchives: [any MTLBinaryArchive]?

An array of binary archives to search for precompiled versions of the shader.

### Specifying Callable Functions for the Pipeline

var vertexLinkedFunctions: MTLLinkedFunctions!

Functions that you can specify as function arguments for the vertex shader when encoding commands that use the pipeline.

var fragmentLinkedFunctions: MTLLinkedFunctions!

Functions that you can specify as function arguments for the fragment shader when encoding commands that use the pipeline.

### Specifying Shader Validation

var shaderValidation: MTLShaderValidation

A value that enables or disables shader validation for the pipeline.

### Instance Properties

var fragmentPreloadedLibraries: [any MTLDynamicLibrary]

var vertexPreloadedLibraries: [any MTLDynamicLibrary]

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

class MTLTileRenderPipelineColorAttachmentDescriptor

A description of a tile-shading render pipeline’s color render target.

struct MTLPipelineOption

Options that determine how Metal prepares the pipeline.

