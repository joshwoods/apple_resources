

- Metal
- MTLRenderPipelineDescriptor
-  sampleCount Deprecated

Instance Property

# sampleCount

The number of samples the pipeline applies for each fragment.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var sampleCount: Int { get set }
```

Deprecated

Use rasterSampleCount instead.

## Discussion

The render pipeline state honors this property only if the pipeline render targets support multisampling.

Important

This property needs to be `1` if the render targets don’t support multisampling.

When your create an MTLRenderCommandEncoder instance, this property’s value needs to be equal to the number of render target textures. Furthermore, the texture type of all render target textures must be MTLTextureType.type2DMultisample.

The number of samples a GPU supports varies by device. You can check whether an MTLDevice instance supports a specific sample count by calling its supportsTextureSampleCount(_:) method.

The default value for this property is `1`.

## See Also

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

