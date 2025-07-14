

- AVFoundation
-  AVVideoExpectedSourceFrameRateKey 

Global Variable

# AVVideoExpectedSourceFrameRateKey

The expected source frame rate.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
let AVVideoExpectedSourceFrameRateKey: String
```

## Discussion

This is not used to control the frame rate; it is provided as a hint to the video encoder so that it can set up internal configuration before compression begins. The actual frame rate depends on frame duration and may vary. This should be set if an auto level AVVideoProfileLevelKey is used, or if the source content has a high frame rate higher than 30 fps. The encoder might have to drop frames to satisfy bit stream requirements if this key is not specified.

## See Also

### Frame rate

let AVVideoAverageNonDroppableFrameRateKey: String

The desired average number of non-droppable frames to be encoded for each second of video.

