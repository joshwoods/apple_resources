

- AVKit
- AVPictureInPictureSampleBufferPlaybackDelegate
-  pictureInPictureController(\_:setPlaying:) 

Instance Method

# pictureInPictureController(\_:setPlaying:)

Tells the delegate that the user requested to begin or pause playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func pictureInPictureController(
    _ pictureInPictureController: AVPictureInPictureController,
    setPlaying playing: Bool
)
```

**Required**

## Parameters 

`pictureInPictureController`  

The Picture in Picture controller.

`playing`  

A Boolean value that indicates whether to begin or pause playback.

## See Also

### Responding to Playback Events

func pictureInPictureControllerTimeRangeForPlayback(AVPictureInPictureController) -> CMTimeRange

Asks the delegate for the current playable time range.

**Required**

func pictureInPictureControllerIsPlaybackPaused(AVPictureInPictureController) -> Bool

Asks delegate to indicate whether the playback UI reflects a playing or paused state, regardless of the current playback rate.

**Required**

func pictureInPictureController(AVPictureInPictureController, didTransitionToRenderSize: CMVideoDimensions)

Tells the delegate when the system Picture in Picture window changes size.

**Required**

func pictureInPictureController(AVPictureInPictureController, skipByInterval: CMTime, completion: () -> Void)

Tells the delegate that the user has requested skipping forward or backward by the indicated time interval.

**Required**

func pictureInPictureControllerShouldProhibitBackgroundAudioPlayback(AVPictureInPictureController) -> Bool

Asks the delegate whether to always prohibit background audio playback.

