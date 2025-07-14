

- Video Toolbox
-  kVTCompressionPropertyKey_MaxKeyFrameInterval 

Global Variable

# kVTCompressionPropertyKey_MaxKeyFrameInterval

The maximum interval between key frames, also known as the key frame rate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MaxKeyFrameInterval: CFString
```

## Discussion

Key frames, also known as sync frames, reset inter-frame dependencies; decoding a key frame is sufficient to prepare a decoder for correctly decoding the difference frames that follow. Video encoders are allowed to generate key frames more frequently if doing so results in more efficient compression. The default key frame interval is 0, which indicates that the video encoder should choose where to place all key frames. A key frame interval of 1 indicates that every frame must be a keyframe, 2 indicates that at least every other frame must be a keyframe, and so on.

This key can be set in conjunction with kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration, which requires a keyframe every *X* frames or every *Y* seconds, whichever comes first.

## See Also

### Frame Dependency

let kVTCompressionPropertyKey_AllowFrameReordering: CFString

A Boolean value that indicates whether frame reordering is enabled.

let kVTCompressionPropertyKey_AllowOpenGOP: CFString

Enables Open GOP (Group Of Pictures) encoding.

let kVTCompressionPropertyKey_AllowTemporalCompression: CFString

A Boolean value indicating whether temporal compression is enabled.

let kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration: CFString

The maximum duration from one key frame to the next in seconds.

