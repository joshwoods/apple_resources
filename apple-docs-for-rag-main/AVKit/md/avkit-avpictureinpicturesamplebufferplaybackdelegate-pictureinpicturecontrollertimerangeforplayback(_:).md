

- AVKit
- AVPictureInPictureSampleBufferPlaybackDelegate
-  pictureInPictureControllerTimeRangeForPlayback(\_:) 

Instance Method

# pictureInPictureControllerTimeRangeForPlayback(\_:)

Asks the delegate for the current playable time range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func pictureInPictureControllerTimeRangeForPlayback(_ pictureInPictureController: AVPictureInPictureController) -> CMTimeRange
```

**Required**

## Parameters 

`pictureInPictureController`  

The Picture in Picture controller.

## Return Value

A CMTimeRange value that defines the content’s time range.

## Discussion

Use the following guidelines when specifying a time range value:

- For live content, return a time range with a duration of positiveInfinity.

- For nonlive content, return a time range that contains the current time of the sample buffer display layer’s timebase.

- When there’s no content to play, return invalid.

The system calls this method whenever you call the invalidatePlaybackState() method, and at other times as it requires.

## See Also

### Responding to Playback Events

func pictureInPictureController(AVPictureInPictureController, setPlaying: Bool)

Tells the delegate that the user requested to begin or pause playback.

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

