

- Video Toolbox
-  kVTVideoEncoderSpecification_EnableLowLatencyRateControl 

Global Variable

# kVTVideoEncoderSpecification_EnableLowLatencyRateControl

Specifies to select an encoder that supports low-latency operation and enables low-latency mode.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+

``` source
let kVTVideoEncoderSpecification_EnableLowLatencyRateControl: CFString
```

## Discussion

Low latency rate control enforces the following behaviors:

- Infinite GOP (all P frames following the beginning IDR).

- No frame reordering (B frame) or looking ahead.

- Only High profiles. The encoder sets the levels automatically.

- Temporal Layer structure.

## See Also

### Encoder Information

let kVTVideoEncoderSpecification_EncoderID: CFString

A key that indicates a particular video encoder to use.

let kVTCompressionPropertyKey_RecommendedParallelizationLimit: CFString

The recommended number of compression sessions to instantiate in a parallel encoding configuration.

let kVTCompressionPropertyKey_RecommendedParallelizedSubdivisionMinimumDuration: CFString

The recommended minimum duration for a given subdivision in a parallel encoding configuration.

let kVTCompressionPropertyKey_RecommendedParallelizedSubdivisionMinimumFrameCount: CFString

The recommended minimum number of video frames for a given subdivision in a parallel encoding configuration.

let kVTCompressionPropertyKey_EnableLTR: CFString

Enables Long Term Reference (LTR) frames during encoding.

let kVTCompressionPropertyKey_EncoderID: CFString

Specifies a particular video encoder by its ID string.

let kVTCompressionPropertyKey_MinAllowedFrameQP: CFString

The minimum allowed encoded frame QP (Quantization Parameter).

let kVTCompressionPropertyKey_MaxAllowedFrameQP: CFString

The maximum allowed encoded frame QP (Quantization Parameter).

let kVTCompressionPropertyKey_PreserveDynamicHDRMetadata: CFString

Specifies whether to preserve dynamic HDR metadata on the input pixel buffer.

let kVTEncodeFrameOptionKey_AcknowledgedLTRTokens: CFString

Enable Long Term Reference (LTR) frames during encoding.

let kVTEncodeFrameOptionKey_ForceLTRRefresh: CFString

A Boolean value that indicates whether to force Long Term Reference (LTR).

let kVTSampleAttachmentKey_RequireLTRAcknowledgementToken: CFString

A number value that contains a unique token for this Long Term Reference (LTR).

let kVTCompressionPropertyKey_SpatialAdaptiveQPLevel: CFString

A value that controls spatial adaptation of the quantization parameter (QP) based on per-frame statistics.

let kVTCompressionPropertyKey_SuggestedLookAheadFrameCount: CFString

A value that requests that the encoder retain the specified number of frames during encoding.

