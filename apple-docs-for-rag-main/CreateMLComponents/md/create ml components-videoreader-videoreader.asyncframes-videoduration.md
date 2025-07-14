

- Create ML Components
- VideoReader
- VideoReader.AsyncFrames
-  videoDuration 

Instance Property

# videoDuration

The video duration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
let videoDuration: CMTime
```

## See Also

### Getting the properties

var count: Int?

The number of frames. For this sequence count is always nil.

let frameSize: CGSize

The frame size.

let nominalFrameRate: Float

The nominal frame rate.

let timescale: CMTimeScale

The timescale of the video track.

let url: URL

The video file URL, used when throwing an error.

