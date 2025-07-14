

- Create ML Components
- VideoReader
- VideoReader.AsyncFrames
-  count 

Instance Property

# count

The number of frames. For this sequence count is always nil.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var count: Int? { get }
```

## See Also

### Getting the properties

let frameSize: CGSize

The frame size.

let nominalFrameRate: Float

The nominal frame rate.

let timescale: CMTimeScale

The timescale of the video track.

let url: URL

The video file URL, used when throwing an error.

let videoDuration: CMTime

The video duration.

