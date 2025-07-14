

- Video Toolbox
-  kVTCompressionPropertyKey_ConstantBitRate 

Global Variable

# kVTCompressionPropertyKey_ConstantBitRate

Requires that the encoder use a Constant Bit Rate algorithm.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_ConstantBitRate: CFString
```

## See Also

### Rate Control

let kVTCompressionPropertyKey_AverageBitRate: CFString

The long-term desired average bit rate in bits per second.

let kVTCompressionPropertyKey_DataRateLimits: CFString

Zero, one, or two hard limits on data rate.

let kVTCompressionPropertyKey_EstimatedAverageBytesPerFrame: CFString

An estimate of the expected size in bytes of a single encoded frame based on the current configuration.

let kVTCompressionPropertyKey_MoreFramesAfterEnd: CFString

A Boolean value indicating whether and how a compression session concatenates frames with other compressed frames to form a longer series.

let kVTCompressionPropertyKey_MoreFramesBeforeStart: CFString

A Boolean value that indicates whether and how a compression session concatenates frames with other compressed frames to form a longer series.

let kVTCompressionPropertyKey_Quality: CFString

The desired compression quality.

let kVTCompressionPropertyKey_TargetQualityForAlpha: CFString

The target quality to use for encoding the alpha channel.

