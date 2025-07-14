

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  init(sampleBufferDisplayLayer:playbackDelegate:) 

Initializer

# init(sampleBufferDisplayLayer:playbackDelegate:)

Creates a content source with a sample buffer display layer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(
    sampleBufferDisplayLayer: AVSampleBufferDisplayLayer,
    playbackDelegate: any AVPictureInPictureSampleBufferPlaybackDelegate
)
```

## Parameters 

`sampleBufferDisplayLayer`  

The sample buffer display layer to show in Picture in Picture.

`playbackDelegate`  

The playback delegate object that responds to Picture in Picture events.

## See Also

### Creating a Content Source

init(playerLayer: AVPlayerLayer)

Creates a content source with a player layer.

init(activeVideoCallSourceView: UIView, contentViewController: AVPictureInPictureVideoCallViewController)

Creates a content source with an active video call.

