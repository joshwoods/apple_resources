

- Video Toolbox
-  kVTCompressionPropertyKey_MaximumRealTimeFrameRate 

Global Variable

# kVTCompressionPropertyKey_MaximumRealTimeFrameRate

A value that specifies the maximum real time rate at which frames can be submitted to a compression session.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let kVTCompressionPropertyKey_MaximumRealTimeFrameRate: CFString
```

## Discussion

The frame rate is measured in frames per second. This property can be used to inform the encoder of the maximum rate that frames could be submitted to the encoder during realtime encoding. This allows the encoder to configure itself to ensure this capability.

This property can only be used when kVTCompressionPropertyKey_RealTime has been set to true.

Unlike kVTCompressionPropertyKey_ExpectedFrameRate, this property informs the maximum possible rate that the compression session could see, not the average frame rate that is expected in normal operation.

By default, the property has a value of zero indicating “unknown”.

## See Also

### Hints

let kVTCompressionPropertyKey_BaseLayerBitRateFraction: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRate: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRateFraction: CFString

let kVTCompressionPropertyKey_ExpectedDuration: CFString

The expected total duration of the compression session, if known.

let kVTCompressionPropertyKey_ExpectedFrameRate: CFString

The expected frame rate, if known.

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

