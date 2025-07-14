

- Video Toolbox
-  kVTCompressionPropertyKey_ExpectedFrameRate 

Global Variable

# kVTCompressionPropertyKey_ExpectedFrameRate

The expected frame rate, if known.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_ExpectedFrameRate: CFString
```

## Discussion

The frame rate is measured in frames per second. This setting is not used to control the frame rate; it’s provided as a hint to the video encoder so that it can set up internal configuration before compression begins. The actual frame rate depends on frame durations and may vary.

By default, this value is `0`, indicating the frame rate is unknown.

## See Also

### Hints

let kVTCompressionPropertyKey_BaseLayerBitRateFraction: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRate: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRateFraction: CFString

let kVTCompressionPropertyKey_ExpectedDuration: CFString

The expected total duration of the compression session, if known.

let kVTCompressionPropertyKey_MaximumRealTimeFrameRate: CFString

A value that specifies the maximum real time rate at which frames can be submitted to a compression session.

let kVTCompressionPropertyKey_PrioritizeEncodingSpeedOverQuality: CFString

A hint for the video encoder to maximize its speed during encoding, sacrificing quality if needed.

let kVTCompressionPropertyKey_ReferenceBufferCount: CFString

let kVTCompressionPropertyKey_SourceFrameCount: CFString

The number of source frames, if known.

let kVTCompressionPropertyKey_CalculateMeanSquaredError: CFString

let kVTCompressionPropertyKey_HasLeftStereoEyeView: CFString

let kVTCompressionPropertyKey_HasRightStereoEyeView: CFString

let kVTCompressionPropertyKey_HorizontalFieldOfView: CFString

let kVTSampleAttachmentKey_QualityMetrics: CFString

let kVTSampleAttachmentQualityMetricsKey_ChromaBlueMeanSquaredError: CFString

let kVTSampleAttachmentQualityMetricsKey_ChromaRedMeanSquaredError: CFString

