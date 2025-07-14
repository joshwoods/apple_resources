

- AVFoundation
-  AVVideoDecompressionPropertiesKey 

Global Variable

# AVVideoDecompressionPropertiesKey

The key that indicates the video decompression properties to pass to the video decoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 10.13+visionOS 1.0+

``` source
let AVVideoDecompressionPropertiesKey: String
```

## Discussion

The value for this key is specified as an NSDictionary object containing other keys to pass to the video decoder.

## See Also

### Compression

let AVVideoCompressionPropertiesKey: String

A key to access the dictionary of compression properties for a video asset.

let AVVideoAverageBitRateKey: String

A key to access the average bit rate—as bits per second—used in compressing video.

let AVVideoQualityKey: String

A key to set the JPEG compression quality of the video.

let AVVideoMaxKeyFrameIntervalKey: String

A key to access the maximum interval between keyframes.

let AVVideoMaxKeyFrameIntervalDurationKey: String

A key to access the maximum interval duration between keyframes.

let AVVideoAllowFrameReorderingKey: String

A key to access permission to reorder frames.

let AVVideoAppleProRAWBitDepthKey: String

A key to access the Apple ProRAW bit depth.

