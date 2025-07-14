

- Metal
- MTLRenderPipelineDescriptor
-  inputPrimitiveTopology 

Instance Property

# inputPrimitiveTopology

The type of primitive topology the pipeline renders.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 14.5+visionOS 1.0+

``` source
var inputPrimitiveTopology: MTLPrimitiveTopologyClass { get set }
```

## Mentioned in 

Rendering to Multiple Texture Slices in a Draw Command

## Discussion

Your app must specify this value when layered rendering is enabled.

The default value is `MTLPrimitiveTopologyClassUnspecified`.

## See Also

### Related Documentation

var renderTargetArrayLength: Int

The number of active layers that all attachments must have for layered rendering.

### Specifying Rasterization and Visibility State

var isAlphaToCoverageEnabled: Bool

A Boolean value that indicates whether to read and use the alpha channel fragment output for color attachments to compute a sample coverage mask.

var isAlphaToOneEnabled: Bool

A Boolean value that indicates whether to force alpha channel values for color attachments to the largest representable value.

var isRasterizationEnabled: Bool

A Boolean value that determines whether the pipeline rasterizes primitives.

var rasterSampleCount: Int

The number of samples the pipeline applies for each fragment.

enum MTLPrimitiveTopologyClass

The primitive topologies available for rendering.

var sampleCount: Int

The number of samples the pipeline applies for each fragment.

Deprecated

