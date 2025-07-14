

- Video Toolbox
-  kVTCompressionPropertyKey_SpatialAdaptiveQPLevel 

Global Variable

# kVTCompressionPropertyKey_SpatialAdaptiveQPLevel

A value that controls spatial adaptation of the quantization parameter (QP) based on per-frame statistics.

macOS 15.0+

``` source
let kVTCompressionPropertyKey_SpatialAdaptiveQPLevel: CFString
```

## Discussion

If set to kVTQPModulationLevel_Disable, spatial QP adaptation is not applied based on per-frame statistics. If set to kVTQPModulationLevel_Default, video encoder is allowed to apply spatial QP adaptation for each macro block (or coding unit) within a video frame. QP adaptation is based on spatial characteristics of a frame and the level of spatial QP adaptation is decided internally by the rate controller.

## Topics

### Levels

var kVTQPModulationLevel_Default: Int

var kVTQPModulationLevel_Disable: Int

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

let kVTCompressionPropertyKey_SuggestedLookAheadFrameCount: CFString

A value that requests that the encoder retain the specified number of frames during encoding.

