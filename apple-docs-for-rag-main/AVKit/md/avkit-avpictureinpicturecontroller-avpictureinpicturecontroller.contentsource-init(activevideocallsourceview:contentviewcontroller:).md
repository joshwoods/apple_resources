

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  init(activeVideoCallSourceView:contentViewController:) 

Initializer

# init(activeVideoCallSourceView:contentViewController:)

Creates a content source with an active video call.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
init(
    activeVideoCallSourceView sourceView: UIView,
    contentViewController: AVPictureInPictureVideoCallViewController
)
```

## Parameters 

`sourceView`  

A view that contains the content of the video call.

`contentViewController`  

The view controller to appear in the system’s Picture in Picture window.

## Discussion

The instance is only valid for the duration of the call.

Important

The use of this API requires an entitlement. For information about requesting access, see com.apple.developer.avfoundation.multitasking-camera-access.

## See Also

### Creating a Content Source

init(playerLayer: AVPlayerLayer)

Creates a content source with a player layer.

init(sampleBufferDisplayLayer: AVSampleBufferDisplayLayer, playbackDelegate: any AVPictureInPictureSampleBufferPlaybackDelegate)

Creates a content source with a sample buffer display layer.

