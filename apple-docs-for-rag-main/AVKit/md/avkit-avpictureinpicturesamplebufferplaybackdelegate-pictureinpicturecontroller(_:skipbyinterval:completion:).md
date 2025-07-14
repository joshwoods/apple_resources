

- AVKit
- AVPictureInPictureSampleBufferPlaybackDelegate
-  pictureInPictureController(\_:skipByInterval:completion:) 

Instance Method

# pictureInPictureController(\_:skipByInterval:completion:)

Tells the delegate that the user has requested skipping forward or backward by the indicated time interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func pictureInPictureController(
    _ pictureInPictureController: AVPictureInPictureController,
    skipByInterval skipInterval: CMTime,
    completion completionHandler: @escaping () -> Void
)
```

``` source
func pictureInPictureController(
    _ pictureInPictureController: AVPictureInPictureController,
    skipByInterval skipInterval: CMTime
) async
```

**Required**

## Parameters 

`pictureInPictureController`  

The Picture in Picture controller.

`skipInterval`  

A doc://com.apple.documentation/documentation/coremedia/cmtime-u58 value that indicates the time interval by which to skip.

`completionHandler`  

You must call the completion handler whether your seek operation succeeds or fails. Failing to call the completion handler is an app error and leaves the user interface in a seeking state.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func pictureInPictureController(_ pictureInPictureController: AVPictureInPictureController, skipByInterval skipInterval: CMTime) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Your app’s implementation of this method may choose to seek by a different interval for efficiency reasons, such as seeking to a particular key frame or only allowing seeks that fall within the playable timeline.

Important

Before calling the completion handler, ensure the seek operation is complete and the timebase reflects the current time and playback rate.

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

func pictureInPictureControllerShouldProhibitBackgroundAudioPlayback(AVPictureInPictureController) -> Bool

Asks the delegate whether to always prohibit background audio playback.

