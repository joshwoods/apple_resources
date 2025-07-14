

- AVKit
- AVPictureInPictureSampleBufferPlaybackDelegate
-  pictureInPictureControllerIsPlaybackPaused(\_:) 

Instance Method

# pictureInPictureControllerIsPlaybackPaused(\_:)

Asks delegate to indicate whether the playback UI reflects a playing or paused state, regardless of the current playback rate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func pictureInPictureControllerIsPlaybackPaused(_ pictureInPictureController: AVPictureInPictureController) -> Bool
```

**Required**

## Parameters 

`pictureInPictureController`  

The Picture in Picture controller.

## Return Value

true to indicate a paused state, otherwise false.

## Discussion

The system calls this method whenever you call its invalidatePlaybackState() method, and at other times as it requires.

## See Also

### Responding to Playback Events

func pictureInPictureController(AVPictureInPictureController, setPlaying: Bool)

Tells the delegate that the user requested to begin or pause playback.

**Required**

func pictureInPictureControllerTimeRangeForPlayback(AVPictureInPictureController) -> CMTimeRange

Asks the delegate for the current playable time range.

**Required**

func pictureInPictureController(AVPictureInPictureController, didTransitionToRenderSize: CMVideoDimensions)

Tells the delegate when the system Picture in Picture window changes size.

**Required**

func pictureInPictureController(AVPictureInPictureController, skipByInterval: CMTime, completion: () -> Void)

Tells the delegate that the user has requested skipping forward or backward by the indicated time interval.

**Required**

func pictureInPictureControllerShouldProhibitBackgroundAudioPlayback(AVPictureInPictureController) -> Bool

Asks the delegate whether to always prohibit background audio playback.

