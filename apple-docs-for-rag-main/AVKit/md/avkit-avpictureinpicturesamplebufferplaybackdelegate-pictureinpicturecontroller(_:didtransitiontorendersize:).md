

- AVKit
- AVPictureInPictureSampleBufferPlaybackDelegate
-  pictureInPictureController(\_:didTransitionToRenderSize:) 

Instance Method

# pictureInPictureController(\_:didTransitionToRenderSize:)

Tells the delegate when the system Picture in Picture window changes size.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func pictureInPictureController(
    _ pictureInPictureController: AVPictureInPictureController,
    didTransitionToRenderSize newRenderSize: CMVideoDimensions
)
```

**Required**

## Parameters 

`pictureInPictureController`  

The Picture in Picture controller.

`newRenderSize`  

The Picture in Picture content’s rendered size, in pixels.

## Discussion

Take the new render size and the isPictureInPictureActive state into account when choosing media variants to avoid uncessary decoding overhead.

## See Also

### Responding to Playback Events

func pictureInPictureController(AVPictureInPictureController, setPlaying: Bool)

Tells the delegate that the user requested to begin or pause playback.

**Required**

func pictureInPictureControllerTimeRangeForPlayback(AVPictureInPictureController) -> CMTimeRange

Asks the delegate for the current playable time range.

**Required**

func pictureInPictureControllerIsPlaybackPaused(AVPictureInPictureController) -> Bool

Asks delegate to indicate whether the playback UI reflects a playing or paused state, regardless of the current playback rate.

**Required**

func pictureInPictureController(AVPictureInPictureController, skipByInterval: CMTime, completion: () -> Void)

Tells the delegate that the user has requested skipping forward or backward by the indicated time interval.

**Required**

func pictureInPictureControllerShouldProhibitBackgroundAudioPlayback(AVPictureInPictureController) -> Bool

Asks the delegate whether to always prohibit background audio playback.

