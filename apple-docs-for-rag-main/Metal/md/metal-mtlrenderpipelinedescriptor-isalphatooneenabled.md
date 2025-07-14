

- Metal
- MTLRenderPipelineDescriptor
-  isAlphaToOneEnabled 

Instance Property

# isAlphaToOneEnabled

A Boolean value that indicates whether to force alpha channel values for color attachments to the largest representable value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var isAlphaToOneEnabled: Bool { get set }
```

## Discussion

The default value is false.

If enabled, alpha channel fragment values are only forced for `colorAttachments[0]`. Other attachments are unaffected.

You may use `alphaToOneEnabled` when you want to write an alpha value that represents partial coverage of the pixel, but also want to disable blending (by forcing alpha to one).

## See Also

### Specifying Rasterization and Visibility State

var isAlphaToCoverageEnabled: Bool

A Boolean value that indicates whether to read and use the alpha channel fragment output for color attachments to compute a sample coverage mask.

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

