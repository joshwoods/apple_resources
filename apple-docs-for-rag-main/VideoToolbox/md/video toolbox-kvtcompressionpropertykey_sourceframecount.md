

- Video Toolbox
-  kVTCompressionPropertyKey_SourceFrameCount 

Global Variable

# kVTCompressionPropertyKey_SourceFrameCount

The number of source frames, if known.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_SourceFrameCount: CFString
```

## Discussion

This property allows a client to give the video encoder advance guidance as to how many frames will be encoded. If nonzero, this value should be the exact number of times that the client calls VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:) in each pass.

The default is `0`, which indicates that the number of source frames is unknown.

## See Also

### Hints

let kVTCompressionPropertyKey_BaseLayerBitRateFraction: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRate: CFString

let kVTCompressionPropertyKey_BaseLayerFrameRateFraction: CFString

let kVTCompressionPropertyKey_ExpectedDuration: CFString

The expected total duration of the compression session, if known.

let kVTCompressionPropertyKey_ExpectedFrameRate: CFString

The expected frame rate, if known.

let kVTCompressionPropertyKey_MaximumRealTimeFrameRate: CFString

A value that specifies the maximum real time rate at which frames can be submitted to a compression session.

let kVTCompressionPropertyKey_PrioritizeEncodingSpeedOverQuality: CFString

A hint for the video encoder to maximize its speed during encoding, sacrificing quality if needed.

let kVTCompressionPropertyKey_ReferenceBufferCount: CFString

let kVTCompressionPropertyKey_CalculateMeanSquaredError: CFString

let kVTCompressionPropertyKey_HasLeftStereoEyeView: CFString

let kVTCompressionPropertyKey_HasRightStereoEyeView: CFString

let kVTCompressionPropertyKey_HorizontalFieldOfView: CFString

let kVTSampleAttachmentKey_QualityMetrics: CFString

let kVTSampleAttachmentQualityMetricsKey_ChromaBlueMeanSquaredError: CFString

let kVTSampleAttachmentQualityMetricsKey_ChromaRedMeanSquaredError: CFString

