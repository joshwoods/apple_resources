

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:willResumePlaybackAfterUserNavigatedFrom:to:) 

Instance Method

# playerViewController(\_:willResumePlaybackAfterUserNavigatedFrom:to:)

Tells the delegate when the user navigates to a new time and playback is about to begin.

tvOS 9.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    willResumePlaybackAfterUserNavigatedFrom oldTime: CMTime,
    to targetTime: CMTime
)
```

## Parameters 

`playerViewController`  

The player view controller.

`oldTime`  

The current playback time before the user began navigating.

`targetTime`  

The new time where playback is about to resume.

## Discussion

Unlike the timeJumpedNotification notification, this method fires only for complete, user-initiated navigation events. For example, if the user begins scrubbing through the media timeline and pauses several times before resuming playback, the player view controller calls this method only once.

You can use this method to present interstitial content before resuming playback, however, it’s recommended to use playerViewController(_:timeToSeekAfterUserNavigatedFrom:to:) for this purpose.

## See Also

### Responding to Navigation Events

func playerViewController(AVPlayerViewController, timeToSeekAfterUserNavigatedFrom: CMTime, to: CMTime) -> CMTime

Tells the delegate when the user skips, scrubs, or otherwise navigates to a new time and wants to resume playback at the target time.

func skipToPreviousItem(for: AVPlayerViewController)

Tells the delegate when the user requests skipping to the previous item in the timeline.

func skipToNextItem(for: AVPlayerViewController)

Tells the delegate when the user requests skipping to the next item in the timeline.

