

- Video Toolbox
-  kVTCompressionPropertyKey_AllowTemporalCompression 

Global Variable

# kVTCompressionPropertyKey_AllowTemporalCompression

A Boolean value indicating whether temporal compression is enabled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_AllowTemporalCompression: CFString
```

## Discussion

The default value is `true`. Set this `value` to false to require key-frame-only compression.

## See Also

### Frame Dependency

let kVTCompressionPropertyKey_AllowFrameReordering: CFString

A Boolean value that indicates whether frame reordering is enabled.

let kVTCompressionPropertyKey_AllowOpenGOP: CFString

Enables Open GOP (Group Of Pictures) encoding.

let kVTCompressionPropertyKey_MaxKeyFrameInterval: CFString

The maximum interval between key frames, also known as the key frame rate.

let kVTCompressionPropertyKey_MaxKeyFrameIntervalDuration: CFString

The maximum duration from one key frame to the next in seconds.

