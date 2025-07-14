

- Create ML Components
- VideoReader
- VideoReader.AsyncFrames
-  frameSize 

Instance Property

# frameSize

The frame size.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
let frameSize: CGSize
```

## See Also

### Getting the properties

var count: Int?

The number of frames. For this sequence count is always nil.

let nominalFrameRate: Float

The nominal frame rate.

let timescale: CMTimeScale

The timescale of the video track.

let url: URL

The video file URL, used when throwing an error.

let videoDuration: CMTime

The video duration.

