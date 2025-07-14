

- Video Toolbox
-  kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration 

Global Variable

# kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration

The maximum duration from one key frame to the next in seconds.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration: CFString
```

## Discussion

The default value is `0`, which means no limit. This property is particularly useful when the frame rate is variable. See kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration for more discussion of key frames.

This key can be set in conjunction with kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration, which requires a keyframe every `X` frames or every `Y` seconds, whichever comes first.

## See Also

### Frame Dependency

let kVTCompressionPropertyKey_AllowFrameReordering: CFString

A Boolean value that indicates whether frame reordering is enabled.

let kVTCompressionPropertyKey_AllowOpenGOP: CFString

Enables Open GOP (Group Of Pictures) encoding.

let kVTCompressionPropertyKey_AllowTemporalCompression: CFString

A Boolean value indicating whether temporal compression is enabled.

let kVTCompressionPropertyKey_MaxKeyFrameInterval: CFString

The maximum interval between key frames, also known as the key frame rate.

