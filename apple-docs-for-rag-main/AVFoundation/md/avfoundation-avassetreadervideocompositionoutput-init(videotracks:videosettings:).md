

- AVFoundation
- AVAssetReaderVideoCompositionOutput
-  init(videoTracks:videoSettings:) 

Initializer

# init(videoTracks:videoSettings:)

Creates an object that reads composited video frames from the specified video tracks.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
init(
    videoTracks: [AVAssetTrack],
    videoSettings: [String : Any]?
)
```

## Parameters 

`videoTracks`  

An array of asset tracks from which to read video frames for compositing. The media type of each track must be video.

`videoSettings`  

Specifying a `nil` value configures the output to return samples in an uncompressed format.

