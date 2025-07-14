

- AVFoundation
-  AVVideoCompressionPropertiesKey 

Global Variable

# AVVideoCompressionPropertiesKey

A key to access the dictionary of compression properties for a video asset.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let AVVideoCompressionPropertiesKey: String
```

## Discussion

The value for this key is an instance of NSDictionary. Add entries to this dictionary to manually change bit rate, B-frame delivery, I-frame interval, and codec quality. Querying the supportedOutputSettingsKeys(for:) method reveals the keys supported for the current release and configuration.

## See Also

### Compression

let AVVideoDecompressionPropertiesKey: String

The key that indicates the video decompression properties to pass to the video decoder.

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

