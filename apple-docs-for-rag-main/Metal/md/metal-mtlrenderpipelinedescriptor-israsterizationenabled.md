

- Metal
- MTLRenderPipelineDescriptor
-  isRasterizationEnabled 

Instance Property

# isRasterizationEnabled

A Boolean value that determines whether the pipeline rasterizes primitives.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var isRasterizationEnabled: Bool { get set }
```

## Discussion

The default value is true, indicating that primitives are rasterized. If the value is false, then primitives are dropped prior to rasterization (i.e. rasterization is disabled). Disabling rasterization may be useful to gather data from vertex-only transformations.

When this value is false, no fragments are processed and the vertex shader function must return `void`.

## See Also

### Specifying Rasterization and Visibility State

var isAlphaToCoverageEnabled: Bool

A Boolean value that indicates whether to read and use the alpha channel fragment output for color attachments to compute a sample coverage mask.

var isAlphaToOneEnabled: Bool

A Boolean value that indicates whether to force alpha channel values for color attachments to the largest representable value.

var inputPrimitiveTopology: MTLPrimitiveTopologyClass

The type of primitive topology the pipeline renders.

var rasterSampleCount: Int

The number of samples the pipeline applies for each fragment.

enum MTLPrimitiveTopologyClass

The primitive topologies available for rendering.

var sampleCount: Int

The number of samples the pipeline applies for each fragment.

Deprecated

