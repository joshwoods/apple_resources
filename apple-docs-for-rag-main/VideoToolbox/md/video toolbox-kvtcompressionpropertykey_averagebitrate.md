

- Video Toolbox
-  kVTCompressionPropertyKey_AverageBitRate 

Global Variable

# kVTCompressionPropertyKey_AverageBitRate

The long-term desired average bit rate in bits per second.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_AverageBitRate: CFString
```

## Discussion

This value is not a hard limit; the bit rate may peak above this. The default bit rate is zero, which indicates that the video encoder should determine the size of compressed data. Note that bit rate settings only have an effect when timing information is provided for source frames, and that some codecs do not support limiting to specified bit rates.

## See Also

### Rate Control

let kVTCompressionPropertyKey_ConstantBitRate: CFString

Requires that the encoder use a Constant Bit Rate algorithm.

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

