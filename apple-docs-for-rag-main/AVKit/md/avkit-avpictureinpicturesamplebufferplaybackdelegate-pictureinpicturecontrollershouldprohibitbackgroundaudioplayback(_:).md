

- AVKit
- AVPictureInPictureSampleBufferPlaybackDelegate
-  pictureInPictureControllerShouldProhibitBackgroundAudioPlayback(\_:) 

Instance Method

# pictureInPictureControllerShouldProhibitBackgroundAudioPlayback(\_:)

Asks the delegate whether to always prohibit background audio playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
optional func pictureInPictureControllerShouldProhibitBackgroundAudioPlayback(_ pictureInPictureController: AVPictureInPictureController) -> Bool
```

## Parameters 

`pictureInPictureController`  

The Picture in Picture controller instance.

## Return Value

true if the delegate prohibits background audio playback; otherwise, false.

## Discussion

If you implement this method, the system calls it once for each invocation of invalidatePlaybackState() to determine whether to prohibit audio playback when the Picture in Picture window is in the background.

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

func pictureInPictureController(AVPictureInPictureController, didTransitionToRenderSize: CMVideoDimensions)

Tells the delegate when the system Picture in Picture window changes size.

**Required**

func pictureInPictureController(AVPictureInPictureController, skipByInterval: CMTime, completion: () -> Void)

Tells the delegate that the user has requested skipping forward or backward by the indicated time interval.

**Required**

