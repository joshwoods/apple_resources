

- Video Toolbox
-  kVTCompressionPropertyKey_MoreFramesAfterEnd 

Global Variable

# kVTCompressionPropertyKey_MoreFramesAfterEnd

A Boolean value indicating whether and how a compression session concatenates frames with other compressed frames to form a longer series.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MoreFramesAfterEnd: CFString
```

## Discussion

This value is `true` if frames compressed in a separate session will be concatenated following the end of the current session. This value is `false` if the current session is a stand-alone session, or if this session will encode the last segment of a multi-segment compression.

The default value is `false`.

## See Also

### Rate Control

let kVTCompressionPropertyKey_AverageBitRate: CFString

The long-term desired average bit rate in bits per second.

let kVTCompressionPropertyKey_ConstantBitRate: CFString

Requires that the encoder use a Constant Bit Rate algorithm.

let kVTCompressionPropertyKey_DataRateLimits: CFString

Zero, one, or two hard limits on data rate.

let kVTCompressionPropertyKey_EstimatedAverageBytesPerFrame: CFString

An estimate of the expected size in bytes of a single encoded frame based on the current configuration.

let kVTCompressionPropertyKey_MoreFramesBeforeStart: CFString

A Boolean value that indicates whether and how a compression session concatenates frames with other compressed frames to form a longer series.

let kVTCompressionPropertyKey_Quality: CFString

The desired compression quality.

let kVTCompressionPropertyKey_TargetQualityForAlpha: CFString

The target quality to use for encoding the alpha channel.

