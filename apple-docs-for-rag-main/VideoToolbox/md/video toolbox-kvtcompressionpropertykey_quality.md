

- Video Toolbox
-  kVTCompressionPropertyKey_Quality 

Global Variable

# kVTCompressionPropertyKey_Quality

The desired compression quality.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_Quality: CFString
```

## Discussion

Some encoders, such as JPEG, describe the compression level of each image with a quality value. This value should be specified as a number in the range of 0.0 to 1.0, where low = 0.25, normal = 0.50, high = 0.75, and 1.0 implies lossless compression for encoders that support it.

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

let kVTCompressionPropertyKey_TargetQualityForAlpha: CFString

The target quality to use for encoding the alpha channel.

