

- Video Toolbox
-  kVTEncodeFrameOptionKey_ForceKeyFrame 

Global Variable

# kVTEncodeFrameOptionKey_ForceKeyFrame

Boolean value indicating whether the current frame is forced to be a key frame.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTEncodeFrameOptionKey_ForceKeyFrame: CFString
```

## Discussion

This value is set in the `frameProperties` dictionary passed to VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:sourceFrameRefcon:infoFlagsOut:); it determines whether the current frame is forced to be a keyframe or not. Note that it may not be possible for the encoder to accommodate all requests.

## See Also

### Per-Frame Configuration

let kVTEncodeFrameOptionKey_BaseFrameQP: CFString

