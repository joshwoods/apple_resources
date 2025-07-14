

- Video Toolbox
-  kVTCompressionPropertyKey_TargetQualityForAlpha 

Global Variable

# kVTCompressionPropertyKey_TargetQualityForAlpha

The target quality to use for encoding the alpha channel.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_TargetQualityForAlpha: CFString
```

## Discussion

Specify this value as a number in the range of `0.0` for the lowest quality to `1.0` for nearly lossless quality. Alpha plane bit rates tend to increase with increasing values. When encoding the alpha channel, the system gives priority to quality over bitrate.

Important

Only HEVC with Alpha encoders support this parameter.

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

let kVTCompressionPropertyKey_MoreFramesAfterEnd: CFString

A Boolean value indicating whether and how a compression session concatenates frames with other compressed frames to form a longer series.

let kVTCompressionPropertyKey_MoreFramesBeforeStart: CFString

A Boolean value that indicates whether and how a compression session concatenates frames with other compressed frames to form a longer series.

let kVTCompressionPropertyKey_Quality: CFString

The desired compression quality.

