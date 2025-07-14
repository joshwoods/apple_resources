

- Video Toolbox
-  kVTCompressionPropertyKey_SuggestedLookAheadFrameCount 

Global Variable

# kVTCompressionPropertyKey_SuggestedLookAheadFrameCount

A value that requests that the encoder retain the specified number of frames during encoding.

macOS 15.0+

``` source
let kVTCompressionPropertyKey_SuggestedLookAheadFrameCount: CFString
```

## Discussion

These frames will be used for additional analysis and statistics gathering before the frame is finally encoded at the end of the window. When this property is not set, video encoder will automatically determine the number of lookahead frames.

Encoder will choose number of lookahead frames closer to the suggested value based on internal configuration. This property directly affects latency of the video encoder. The following properties also affect look ahead frames:

1.  Value of this property must be less than or equal to `kVTCompressionPropertyKey_MaxFrameDelayCount`.

2.  This property is ignored when `VTVideoEncoderSpecification_EnableLowLatencyRateControl` is set to true

3.  This property is ignored when `kVTCompressionPropertyKey_Quality` is set to 1.0

4.  This property can not be used in conjunction with multi-pass feature (`kVTCompressionPropertyKey_MultiPassStorage`)

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

let kVTVideoEncoderSpecification_EnableLowLatencyRateControl: CFString

Specifies to select an encoder that supports low-latency operation and enables low-latency mode.

let kVTCompressionPropertyKey_SpatialAdaptiveQPLevel: CFString

A value that controls spatial adaptation of the quantization parameter (QP) based on per-frame statistics.

