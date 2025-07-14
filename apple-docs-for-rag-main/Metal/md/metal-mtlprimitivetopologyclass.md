

- Metal
-  MTLPrimitiveTopologyClass 

Enumeration

# MTLPrimitiveTopologyClass

The primitive topologies available for rendering.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 12.0+visionOS 1.0+

``` source
enum MTLPrimitiveTopologyClass
```

## Topics

### Constants

case unspecified

An unspecified primitive.

case point

A point primitive.

case line

A line primitive.

case triangle

A triangle primitive.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var sampleCount: Int

The number of samples the pipeline applies for each fragment.

Deprecated

