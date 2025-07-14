

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  init(playerLayer:) 

Initializer

# init(playerLayer:)

Creates a content source with a player layer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(playerLayer: AVPlayerLayer)
```

## Parameters 

`playerLayer`  

The player layer to show in Picture in Picture.

## See Also

### Creating a Content Source

init(sampleBufferDisplayLayer: AVSampleBufferDisplayLayer, playbackDelegate: any AVPictureInPictureSampleBufferPlaybackDelegate)

Creates a content source with a sample buffer display layer.

init(activeVideoCallSourceView: UIView, contentViewController: AVPictureInPictureVideoCallViewController)

Creates a content source with an active video call.

